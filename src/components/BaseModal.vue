<script setup>
import { ref } from 'vue'

defineProps({
  modalActive: {
    type: Boolean,
    default: false
  }
})
defineEmits(['close-modal'])
</script>

<template>
  <Transition name="modal-outer">
    <div
      v-show="modalActive"
      @click="$emit('close-modal')"
      class="fixed w-full bg-black bg-opacity-50 z-[10] h-screen top-0 left-0 flex justify-center px-8"
    >
      <Transition name="modal-inner">
        <div
          v-if="modalActive"
          class="px-[62px] py-[49px] bg-white self-start mt-32 max-w-screen-md rounded-lg"
        >
          <slot />
        </div>
      </Transition>
    </div>
  </Transition>
</template>

<style>
.modal-outer-enter-active,
.modal-outer-leave-active {
  transition: opacity 0.3s cubic-bezier(0.52, 0.02, 0.19, 1.02);
}

.modal-outer-enter-from,
.modal-outer-leave-to {
  opacity: 0;
}
</style>
