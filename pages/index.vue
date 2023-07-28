<script setup>
useHead({
  title: 'Home Page',
  script: ['main.js'],
  meta: [{ name: 'description', content: 'This website is about nuxtjs' }],
});

const { data } = useFetch('/api/userdetails');
</script>
<template>
  <h1>Home Page</h1>
  <p>{{ data.msg }}</p>
  <NuxtLink to="/about">Goto about page</NuxtLink>
</template>
