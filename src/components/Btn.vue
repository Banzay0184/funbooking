<script setup>
defineProps({
  styleBtn: String
})
</script>

<template>
  <button :class="styleBtn"><slot /></button>
</template>

<style scoped>
.btn-normal {
  border-radius: 7px;
  padding: 6px 10px;
  width: 200px;
  background: #2b64c8;
  color: white;
}

.btn-normal:hover {
  background: #0d46aa;
}


.btn-icon {
  border-radius: 7px;
  padding: 10px 47px;
  background: #2b64c8;
  color: white;
}

.btn-icon:hover {
  background: #0d46aa;
}

.btn-line {
  padding: 10px 0;
  border-radius: 7px;
  padding: 6px 10px;
  width: 200px;
  border: 1px solid #2b64c8;
  color: #2b64c8;
}

.btn-line:hover {
  box-shadow: 0 1px 6px 0 rgba(43, 100, 200, 0.54);
  background: #fff;
}
</style>
