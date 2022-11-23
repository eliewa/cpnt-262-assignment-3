<script setup>
import { RouterLink, RouterView } from "vue-router";
import AppNavBarVue from "../src/components/AppNavBar.vue"
</script>

<template>
  <header>
    <AppNavBarVue />  
  </header>

  <RouterView />
</template>
