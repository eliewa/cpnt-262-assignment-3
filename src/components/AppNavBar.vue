
<script setup>
import { RouterLink, RouterView } from "vue-router";
const props = defineProps ({
    product: {
      default: "Products",
      type: String,
    },
    contact: {
      default: "Contact",
      type: String,
    },

    about: {
      default: "About",
      type: String,
    },

    home: {
      default: "Home",
      type: String,
    },

    image: {
      default: "src/assets/images/batman.jpg",
      type: String
    },

    alt: {
      default: "Batman Image",
      type: String,
    },
  })
</script>

<template>
  <header class="flex justify-center gap-14 text-lg font-bold bg-gray-900 text-white p-5">
    <RouterLink to="/">{{home}}</RouterLink>
    <RouterLink to="/about">{{about}}</RouterLink>
    <p>{{product}}</p>
    <p>{{contact}}</p>
  </header>
</template>