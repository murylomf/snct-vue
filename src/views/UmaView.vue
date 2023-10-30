<template>
    <div id="msg">{{ msg }}</div>
    <button @click="testeClick()">Botão</button>
</template>
<script setup>
import { onMounted, onBeforeMount, ref } from 'vue'

const msg = ref('Antenor')

function testeClick() {
    msg.value = 'Igor'
}

onMounted(() => {
    console.log('Mounted')
})

onBeforeMount(() => {
    console.log('Antes de montar')
})
</script>
<style></style>