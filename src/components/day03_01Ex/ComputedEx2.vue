<script setup>
import { computed, reactive, ref } from 'vue';

const refCount = ref(0);
const reactiveCount = reactive({ count: 0 });

// ref() 데이터를 활용시 value 속성 사용
const refDoubleCount = computed(() => refCount.value * 2);
// reactive() 데이터는 value 속성 필요 없음
const reactiveDoubleCount = computed(() => reactiveCount.count * 2);

setTimeout(() => {
  refCount.value = 5;
  console.log(refDoubleCount.value);
  reactiveCount.count = 10;
  console.log(reactiveDoubleCount.value);
}, 1000);
</script>

<template>
  <h1>{{ refDoubleCount }}</h1>
  <h1>{{ reactiveDoubleCount }}</h1>
</template>
