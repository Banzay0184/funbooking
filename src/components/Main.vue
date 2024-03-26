<script setup>
import Main from './Btn.vue'
import NewCard from './NewCard.vue'
</script>

<template>
  <div class="overflow-hidden">
    <div class="max-w-[1160px] m-auto px-[20px]">
      <!-- news -->
      <div class="mb-[105px]">
        <h1 class="text-[40px] uppercase mb-[20px]">новости</h1>
        <div class="flex gap-[20px] overflow-x-scroll no-scrollbar">
          <NewCard imageUrl="/seat1.png" title="Как правильно спланировать авиарейс и узнать его стоимость?" text="Всего за несколько часов на самолете можно преодолеть расстояние в тысячи километров и при этом совершенно..."/>
          <NewCard imageUrl="/seat2.png" title="Заказ авиабилетов по интернету - легкий способ путешествовать по миру" text="Распространенной проблемой, связанной с поездкой в другие страны становится невозможность найти ..."/>
          <NewCard imageUrl="/seat3.png" title="Увлекательные туры в Доминикану - мечта любого путешественника" text="После однообразного отдыха в Турции, осмотра статуй фараонов в Египте и круглосуточной пляжной жизни..."/>
          <NewCard imageUrl="/seat1.png" title="Увлекательные туры в Доминикану - мечта любого путешественника" text="После однообразного отдыха в Турции, осмотра статуй фараонов в Египте и круглосуточной пляжной жизни..."/>
        </div>
      </div>
      <!-- stock -->
      <div class="relative flex gap-[20px] mb-[12px] items-center">
        <div class="mr-[20px]">
          <h1 class="text-[36px] font-bold capitalize">Акции</h1>
          <a class="uppercase tracking-wider text-[#2b64c8] flex gap-[6px] items-center" href=""
            >все акции
            <svg
              width="21"
              height="8"
              viewBox="0 0 21 8"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M20.3536 4.35355C20.5488 4.15829 20.5488 3.84171 20.3536 3.64645L17.1716 0.464466C16.9763 0.269204 16.6597 0.269204 16.4645 0.464466C16.2692 0.659728 16.2692 0.976311 16.4645 1.17157L19.2929 4L16.4645 6.82843C16.2692 7.02369 16.2692 7.34027 16.4645 7.53553C16.6597 7.7308 16.9763 7.7308 17.1716 7.53553L20.3536 4.35355ZM0 4.5H20V3.5H0V4.5Z"
                fill="#2B64C8"
              />
            </svg>
          </a>
        </div>
        <img class="drop-shadow-xl w-[550px] h-[250px]" src="/Rectangle74.png" alt="" />
        <div class="drop-shadow-xl bg-white rounded-lg">
          <h3 class="bg-[#2b64c8] p-[15px] rounded-t-lg font-medium text-white">
            Дешевые авиабилеты в Дубай...
          </h3>
          <div class="p-[15px]">
            <div class="flex items-center gap-[42px]">
              <p class="text-[#151515] w-[178px]">Дешевые авиабилеты в Дубай</p>
              <img class="w-[135px]" src="/image 10.png" alt="" />
            </div>
            <div class="flex pb-[15px] gap-[42px] items-end">
              <p class="text-[#7C7C7C]">Стоимость билетов</p>
              <h3 class="text-[24px] font-medium tracking-wider">
                <span class="text-[16px] font-normal tracking-[0.02]">от</span> 25 000 руб.
              </h3>
            </div>
            <button
              class="border-[1px] border-[#2b64c8] border-solid rounded-lg py-[15px] w-[100%] text-center"
            >
              Подробнее
            </button>
          </div>
        </div>
        <img
          class="absolute z-[-2] l-[0] h-[339px] top-[-200px] left-[-400px]"
          src="/Frame-A.png"
          alt=""
        />
      </div>
      <div class="flex mb-[100px] gap-[6px] justify-end">
        <svg
          width="29"
          height="29"
          viewBox="0 0 29 29"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle cx="14.5" cy="14.5" r="14" stroke="#2B64C8" />
          <path d="M17 20L11 14.5L17 9" stroke="#2B64C8" />
        </svg>
        <svg
          width="29"
          height="29"
          viewBox="0 0 29 29"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <circle cx="14.5" cy="14.5" r="14.5" fill="#2B64C8" />
          <path d="M12 9L18 14.5L12 20" stroke="white" />
        </svg>
      </div>
      <!-- InfoBanner -->
      <div class="flex relative items-center h-[200px] mb-[100px]">
        <h1 class="absolute w-[535px] text-[36px] capitalize font-[100] text-[#7C7C7C]">
          Дешевые авиабилеты онлайн – ваши мечты сбудутся
        </h1>
        <img class="absolute right-[-250px] w-[758px]" src="/plane-large.png" alt="" />
      </div>
    </div>
  </div>
</template>
