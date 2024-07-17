<script setup>
  import { ref } from 'vue';

  let colorClass = 'fuga';
  const titleClass = ref(colorClass);
  const dynamicId = ref('hoge');

  setTimeout(() => {
    console.log('3秒経過しました');
    colorClass = 'hoge';
  }, 3000);
</script>

<template>
  <h1 :class="titleClass">Make me red</h1>
  <div :id="dynamicId">hogehoge</div>
</template>

<style>
  .fuga {
    color: blue;
  }
</style>
