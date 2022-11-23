<script setup>
const props = defineProps ({
    text: {
      type: String,
      default: "Search for your favourite Movies:",
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
  <p class="text-white text-2xl font-serif p-10">{{text}}</p>
  <img :src="image" :alt="alt">
  <slot></slot>
</template>

