<script setup>
import { ref } from 'vue';

const inputRef = ref(null);

// 1초 뒤 콜백함수를 실행
setTimeout(() => {
  // h1 태그에 해당하는 DOM 객체
  console.log(inputRef.value);

  // DOM 객체의 속성, 메서드 모두 사용
  console.log(inputRef.value.innerText);
}, 1000);
</script>

<template>
  <h1 ref="inputRef">Hello, Ref!</h1>
</template>
