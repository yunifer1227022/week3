<script setup>
// import { RouterLink, RouterView } from 'vue-router'
import NavbarComponent from './components/NavbarCom.vue'
import FooterComponent from './components/FooterCom.vue'
</script>

<template>
  <NavbarComponent />
  <h2>中間區域</h2>
  <RouterView />
  <FooterComponent />
</template>

<style scoped></style>
