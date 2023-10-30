<template>
    <div> {{ msg }}</div>
    <button @click="testeBtn()">Botão</button>
</template>
<script setup>
import { onMounted, onBeforeMount, ref } from 'vue'
const msg = ref('qualquer coisa')

function testeBtn() {
    msg.value = 'outra coisa'
}

onMounted(() => {
    console.log('Mounted')
})

onBeforeMount(() => {
    console.log('Antes de montar')
})
</script>