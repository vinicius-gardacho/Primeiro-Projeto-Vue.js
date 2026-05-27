<script setup>
  import Titulo from './components/Titulo.vue'
  import ListaTimes from './components/ListaTimes.vue'
  import CartaoTime from './components/CartaoTime.vue'
</script>

<template>
  <Titulo />
  <ListaTimes />
  <CartaoTime times = "Santos" comp = "Sulamericana" />
</template>

<style scoped></style>
