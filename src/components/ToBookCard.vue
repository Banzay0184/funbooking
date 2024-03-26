<script setup>
import Btn from './Btn.vue'
</script>

<template>
  <div class="flex flex-col items-center gap-[15px]">
    <h1 class="font-black text-center w-[600px] uppercase text-[26px]">
      бронирование авиабилетов и отелей на срок до 14 дней.
    </h1>
    <h1 class="font-black text-center uppercase text-[20px] mb-[54px]">
      страховые полисы стран евросоюза
    </h1>
    <div class="flex flex-col gap-[54px] items-center">
      <div class="rounded-[100px] p-[7px] bg-[#2b64c8]">
        <button class="rounded-[100px] p-[7px] bg-white w-[138px] py-[8px] text-black">
          Авиабилеты
        </button>
        <button class="rounded-[100px] p-[7px] w-[138px] py-[8px] text-white">Отели</button>
        <button class="rounded-[100px] p-[7px] w-[138px] py-[8px] text-white">
          Страхование ЕС
        </button>
      </div>
      <div class="relative flex gap-[6px] items-end bg-black/40 pt-[10px] pl-[20px] pr-[20px] pb-[20px] rounded-lg">
        <div class="w-[270px]">
          <h3 class="text-white mb-[4px]">Поездка</h3>
          <div class="rounded-lg p-[12px] bg-white flex gap-[35px]">
            <div class="text-black flex gap-[8px]">
              <p class="text-[12px] text-[#b9b9b9]">откуда</p>
              <select class="text-[12px]">
                <option class="text-[12px]" value="">Москва</option>
              </select>
            </div>
            <div class="text-black flex gap-[8px]">
              <p class="text-[12px] text-[#b9b9b9]">куда</p>
              <select class="text-[12px] mr-[20px]">
                <option class="text-[12px]" value="">Дубай</option>
              </select>
            </div>
          </div>
        </div>
        <svg
        class="absolute left-[275px] top-[43%]"
          width="34"
          height="34"
          viewBox="0 0 34 34"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle
            cx="17"
            cy="17"
            r="16.4632"
            fill="white"
            stroke="#2B64C8"
            stroke-width="1.07368"
          />
          <path
            d="M20.943 10.3786L24.3372 13.7728M24.3372 13.7728L20.943 17.1671M24.3372 13.7728H9.30566"
            stroke="#2B64C8"
            stroke-width="0.969779"
          />
          <path
            d="M12.6996 23.9692L9.30533 20.575M9.30533 20.575L12.6996 17.1807M9.30533 20.575H24.3369"
            stroke="#2B64C8"
            stroke-width="0.969779"
          />
        </svg>
        <div class="w-[100%]">
          <h3 class="text-white mb-[4px]">Поездка</h3>
          <div class="rounded-lg p-[12px] bg-white flex gap-[9px]">
            <div class="text-black flex gap-[8px]">
              <p class="text-[12px] text-[#b9b9b9] ml-[15px]">туда</p>
              <input class="text-[12px]" type="date" />
            </div>
            <div class="text-black flex gap-[8px]">
              <p class="text-[12px] text-[#b9b9b9]">куда</p>
              <input class="text-[12px]" type="date" />
            </div>
          </div>
        </div>

        <div class="w-[100%]">
          <h3 class="text-white mb-[4px]">Пассажиры и класс</h3>
          <div class="rounded-lg p-[12px] bg-white flex gap-[9px]">
            <div class="text-black flex gap-[8px]">
              <p class="text-[12px] text-[#b9b9b9]">туда</p>
              <input
                class="text-[12px] w-[20px] focus:]"
                type="number"
                min="1"
                max="99"
                minlength="1"
                value="1"
              />
            </div>
            <div class="text-black flex gap-[8px]">
              <p class="text-[12px] text-[#b9b9b9]">класс</p>
              <select class="text-[12px]">
                <option class="text-[12px]" value="">Эконом</option>
              </select>
            </div>
          </div>
        </div>

        <Btn styleBtn="btn-icon">Найти</Btn>
      </div>
    </div>
  </div>
</template>
