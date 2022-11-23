<script setup>
  const links = [{item: 'Home'}, {item: 'Products'}, {item: 'About'},
                {item: 'Contact Us'}
  ]
</script>

<template>
  <footer class="text-xl text-white bg-gray-900 mt-auto h-auto p-5">
    <ul class="flex justify-center gap-10">
      <li v-for="link in links">
        {{link.item}}
      </li>
    </ul>
    <p class="text-center p-5 text">&copy; 2012 FilmJunkies inc.</p>
  </footer>

</template>