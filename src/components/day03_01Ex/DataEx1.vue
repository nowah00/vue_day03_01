<script setup>
import { ref } from 'vue';

const count = ref(0); // 기본 자료형 사용
const state = ref({ count: 0 }); // 반응형 데이터

console.log(count.value);
console.log(state.value.count);

// 기본값을 변경을 감지해서 Dom을 업데이트
setTimeout(() => {
  count.value++;
}, 1000);

// 반응형은 변경을 감지 못해 업데이트하지 못함
setTimeout(() => {
  state.count++;
}, 1000);
</script>

<template>
  <!-- 기본값 -->
  <h1>count : {{ count }}</h1>

  <!-- 객체값 -->
  <h1>state : {{ state.count }}</h1>
</template>
