<script setup>
import { ref } from 'vue'
import BaseModal from './BaseModal.vue'
import ToBookCard from './ToBookCard.vue'
import Btn from './Btn.vue'

const modalActive = ref(null)

const toggleModal = () => {
  modalActive.value = !modalActive.value
}


defineProps({
  minActive: {
    type: Boolean,
    default: false
  }
})

const minModalActive = ref(null)
const toggleMinModal = () => {
  minModalActive.value = !minModalActive.value
}
defineEmits(['close-m'])

</script>

<template>
  <div class="">
    <header class="relative bg-[#2b64c8] overflow-x-hidden">
      <div class="max-w-[1160px] m-auto px-[20px] pt-[18px] relative z-10">
        <div
          class="cursor-pointer flex justify-between border-4 px-[45px] border-solid border-white rounded-[34px] mb-[94px]"
        >
          <img class="w-[99px h-[99px]" src="/logo 1.png" alt="logo" />
          <div class="flex items-center gap-[14px] relative">
            <svg
              class="fill-white"
              width="36"
              height="36"
              viewBox="0 0 36 36"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M6 36C6 36 3 36 3 33C3 30 6 21 18 21C30 21 33 30 33 33C33 36 30 36 30 36H6ZM18 18C20.3869 18 22.6761 17.0518 24.364 15.364C26.0518 13.6761 27 11.3869 27 9C27 6.61305 26.0518 4.32387 24.364 2.63604C22.6761 0.948212 20.3869 0 18 0C15.6131 0 13.3239 0.948212 11.636 2.63604C9.94821 4.32387 9 6.61305 9 9C9 11.3869 9.94821 13.6761 11.636 15.364C13.3239 17.0518 15.6131 18 18 18Z"
              />
            </svg>
            <p class="text-white">Личный кабинет</p>
            <svg
              @click="toggleMinModal"
              class="fill-white"
              width="40"
              height="22"
              viewBox="0 0 40 22"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect width="40" height="4" rx="2" />
              <rect y="9" width="40" height="4" rx="2" />
              <rect y="18" width="40" height="4" rx="2" />
            </svg>
            <Transition name="modal-outer">
              <div
                v-show="minModalActive"
                @click="$emit('close-m')"
                class="absolute p-[12px] bg-white rounded-lg flex flex-col gap-[8px] top-[75px] right-0"
              >
                <Transition name="modal-inner">
                  <div v-if="minModalActive" class="">
                    <Btn @click="toggleModal" styleBtn="btn-normal">Войти</Btn>
                    <Btn styleBtn="btn-line">Регистрация</Btn>
                  </div>
                </Transition>
              </div>
            </Transition>
          </div>
        </div>
        <div class="text-[#ffff] p-[50px] flex justify-start flex-col items-center rounded-[58px] w-[100%] h-[522px;] bg-black/40 mb-[43px]">
          <ToBookCard/>
        </div>
      </div>
      <img class="absolute top-[222px] left-[20px] h-[461px]" src="/Frame-L.png" alt="air" />
      <img class="absolute top-[222px] right-[-300px] h-[461px]" src="/Frame-L.png" alt="air" />
    </header>
    <BaseModal :modalActive="modalActive" @close-modal="toggleModal">
      <h1 class="tetx-[#3d3d3d]">hello</h1>
    </BaseModal>
  </div>
</template>
