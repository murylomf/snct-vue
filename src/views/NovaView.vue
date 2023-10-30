<template>
  <div>{{ el }}</div>
  <div>{{ num }}</div>
  <button @click="num++">my button</button>
</template>

<style></style>

<script setup>
import { ref, onMounted, onBeforeMount } from 'vue'

const el = ref('mu')
const num = ref(0)

// onMounted(() => {
//   console.log('Mounted')
//   el.value = 'Teste onMounted'
// })

// onBeforeMount(()=> {
//  console.log('Antes de montar')
// })
</script>
