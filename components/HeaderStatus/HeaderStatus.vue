<template>
  <div :class="{'full-height': fullHeight}" class="header">
    <img src="@/assets/images/logo.jpg" />
    <button @click="expand">Enviar Avaliação</button>
  </div>
</template>
<script setup>
import { ref } from 'vue'
const fullHeight = ref(false)
const expand = () => {
  fullHeight.value = !fullHeight.value
}
</script>
<style src="./HeaderStatus.css" scoped />
