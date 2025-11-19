<script setup>
import DataEx1 from './components/day03_01Ex/DataEx1.vue';
import DataEx2 from './components/day03_01Ex/DataEx2.vue';
import DataEx3 from './components/day03_01Ex/DataEx3.vue';
import DataEx4 from './components/day03_01Ex/DataEx4.vue';
import RefEx1 from './components/day03_01Ex/RefEx1.vue';
import RefEx2 from './components/day03_01Ex/RefEx2.vue';
import ComputedEx1 from './components/day03_01Ex/ComputedEx1.vue';
import ComputedEx2 from './components/day03_01Ex/ComputedEx2.vue';
import LowerUpperCaseEx from './components/exVue/LowerUpperCaseEx.vue';
import SearchByKeyword from './components/exVue/SearchByKeyword.vue';
import TotalOrAvg from './components/exVue/TotalOrAvg.vue';
import GetterSetter from './components/exVue/GetterSetter.vue';
import CheckBoxSelectCount from './components/exVue/CheckBoxSelectCount.vue';

components: {
  DataEx1,
    DataEx2,
    DataEx3,
    DataEx4,
    RefEx1,
    RefEx2,
    ComputedEx1,
    ComputedEx2,
    LowerUpperCaseEx,
    SearchByKeyword,
    TotalOrAvg,
    GetterSetter,
    CheckBoxSelectCount;
}
</script>

<template>
  <!-- <DataEx1 />
  <DataEx2 />
  <DataEx3 />
  <DataEx4 />
  <RefEx1 />
  <RefEx2 />
  <ComputedEx1 />
  <ComputedEx2 /> -->
  <h3>1) 문자열 대문자·소문자 변환</h3>
  <LowerUpperCaseEx />
  <br />

  <h3>2) 배열 검색 필터 기능</h3>
  <SearchByKeyword />
  <br />

  <h3>3) 숫자 합계·평균 계산</h3>
  <TotalOrAvg />
  <br />

  <h3>4) getter / setter 사용한 computed</h3>
  <GetterSetter />
  <br />

  <h3>​5)체크박스 선택 개수에 따른 메시지</h3>
  <CheckBoxSelectCount />
  <br />
</template>
