<script setup>
  const props = defineProps ({
    title: {
      type: String,
      default: "Batman",
    },

    date: {
      type: Number,
      default: 2022,
    },
  })

  const items = [{title: 'Batman', date: 2022}, {title: 'Avatar', date: 2004}, {title: 'Titanic', date: 1997}];
</script>

<template>
  <ul>
    <li v-for="item in items" >
      {{item.title}}
      ({{item.date}})
    </li>
  </ul>
</template>