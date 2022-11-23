<script setup>
import { ref } from 'vue';
import AppHeaderVue from '../components/icons/AppHeader.vue';
import AppListVue from '../components/AppList.vue';
import AppCardVue from '../components/AppCard.vue';
import AppFooterVue from "../components/AppFooter.vue";
</script>

<template>
  <body class="min-h-screen flex flex-col overflow-hidden">
    <main>
    <div class="hero text-white flex flex-col items-center justify-center">
      <div></div>
      <AppHeaderVue
        text="Search millions of movies on our database:"
        image="src/assets/images/avatar.jpg"
        alt="Avatar"
      >
       Avatar (2004)
      </AppHeaderVue>
      <div class="bg-black p-5 mt-2">
        <AppListVue/>
      </div>
      
    </div>

    <section>
      <AppCardVue/>
    </section>
    
  </main>

    <AppFooterVue/>

  </body>
  
</template>
<style>
  .hero {
    background-image: linear-gradient(rgba(0, 0, 0, 0.664), rgba(0, 0, 0, 0.616)), url(../assets/images/andor.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 70vh;
    width: 100%;
  }
</style>