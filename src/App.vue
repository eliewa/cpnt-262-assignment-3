<script setup>
import { RouterLink, RouterView } from "vue-router";
import AppNavBarVue from "./components/icons/AppNavBar.vue";
</script>

<template>
  <header>
    <AppNavBarVue />  
  </header>

  <RouterView />
</template>
