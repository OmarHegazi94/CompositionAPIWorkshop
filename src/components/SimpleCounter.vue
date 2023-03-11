<script setup>
import { ref } from 'vue'
const count = ref(0)

function increase() {
  count.value++
}

function decrease() {
  count.value--
}
</script>

<template>
  <h1>Count: {{ count }}</h1>
  <div>
    <button @click="increase">Increase</button>
    <button @click="decrease">Decrease</button>
  </div>
</template>