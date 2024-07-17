<script setup>
  import { ref } from 'vue';

  const count = ref(0);

  function increment() {
    count.value++;
  }
</script>

<template>
  <button @click="increment">Count is: {{ count }}</button>
  <h1>Title</h1>
</template>
