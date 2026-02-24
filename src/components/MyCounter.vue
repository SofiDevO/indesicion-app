<script setup lang="ts">
import { computed, ref } from 'vue';

const counter = ref(10)
const squareCounter = computed(() => counter.value * counter.value)
</script>

<template>
  <section>
    <h3>Counter:{{ counter }}</h3>
    <h3>square:{{ squareCounter }}</h3>
  </section>
  <button @click="counter++ ">+1</button>
  <button @click="counter-- ">-1</button>
</template>
