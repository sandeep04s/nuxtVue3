<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtWelcome />
    <h2>Hello</h2>
    <button @click="increment">Increment</button>
    <p>Count: {{ count }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const count = ref(0);

const increment = () => {
  count.value++;
};            
</script>

<style scoped>
</style>