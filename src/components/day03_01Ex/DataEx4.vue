<script setup>
import { reactive } from 'vue';

const state = reactive(0);

setTimeout(() => {
  state.value++;
}, 1000);
</script>

<template>
  <h1>state : {{ state.value }}</h1>
</template>
