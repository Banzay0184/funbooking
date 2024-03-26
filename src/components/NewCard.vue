<script setup>
defineProps({
  imageUrl: String,
  title: String,
  text: String,
})
</script>

<template>
  <div class="bg-white rounded-lg drop-shadow-xl p-[20px] min-w-[360px]">
    <img class="" :src="imageUrl" alt="" />
    <h3 class="text-[#2b64c8] font-medium mt-[12px]">
      {{title}}
    </h3>
    <p class="tracking-[0.02] text-[#7C7C7C] mt-[12px]">
     {{text}}
    </p>
  </div>
</template>
