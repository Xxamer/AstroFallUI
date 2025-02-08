<template>
  <div @click="changeVariable" class="alert">
    This is made with Vue loading on astro
  </div>
</template>
<script setup>
import { ref, onMounted } from "vue";
onMounted(() => {
  console.log("Mounted");
});
const test = ref("test");
const changeVariable = () => {
  test.value = "hola";
};
</script>
