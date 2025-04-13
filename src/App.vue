<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <main class="dark:bg-white dark:text-black">
    <nav-bar></nav-bar>
  <RouterView />
  <Footer></Footer>
  </main>
</template>

<style>
.cinzel {
  font-family: "Cinzel", serif;
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
}
</style>