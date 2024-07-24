<script setup>
// 要使用任何方法要 Import module 進來
import { ref } from 'vue';

/* Step1: 定義一個值 */
const num = ref(2);
console.log(num.value);


/* Step2: 操作: 針對這個值要做什麼事情 不會操作畫面 */
function clickMe() {
  num.value++;
}

// 不需要寫 return

</script>

<template>
  <div>
    {{ num }}
    <button type="button" v-on:click="clickMe">點我</button>
  </div>
</template>