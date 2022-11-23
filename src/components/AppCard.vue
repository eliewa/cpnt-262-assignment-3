<script setup>
  const movies = [{image: 'src/assets/images/batman.jpg', title: 'Batman (2022)'},
              {image: 'src/assets/images/andor.jpg', title: 'Andor (2022)'},
              {image: 'src/assets/images/titanic.jpg', title: 'Titanic (1997)'}
  
  ];
</script>

<template>
  <article>
    <ul class="flex justify-center pt-10 pb-10">
      <li class="w-56 h-auto" v-for="movie in movies">
        <img class= "h-56" :src="movie.image" alt="">
        <h1 class="font-bold">{{movie.title}}</h1>
      </li>
    </ul>
  </article>
  
</template>