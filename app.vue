<template>
  <div>
    <h1>{{ ssr }}</h1>
    <NuxtWelcome />
  </div>
</template>

<script setup>
import { ref }  from 'vue';
const ssr = ref("Nö");
if (!process.client){
  ssr.value = "Juhuhuuuuu"
}
</script>
