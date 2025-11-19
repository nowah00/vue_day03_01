<script setup>
import { ref } from 'vue';

// 배열로 반응형 데이터를 생성
const arr1 = ref([10]);
const arr2 = ref([10]);

setTimeout(() => {
  arr1.value = [10, 20]; // 배열의 값 자체를 변경
}, 1000);

setTimeout(() => {
  arr2.push = [20]; // 배열의 요소 변경 (추가)
}, 1000);

// 기본값이나 값 자체를 변경하는 것은 감지가 가능하여 리턴 가능하지만,
//  요소를 변경하는 것은 감지 할 수 없다.
</script>

<template>
  <h1>arr1 : {{ arr1 }}</h1>
  <h1>arr2 : {{ arr2 }}</h1>
</template>
