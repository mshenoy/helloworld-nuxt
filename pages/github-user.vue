<script setup>
const { data: user } = useFetch('https://api.github.com/users/mshenoy');
</script>
<template>
  <h1>{{ user?.name }}</h1>
  <p>{{ user?.blog }}</p>
  <p>{{ user?.bio }}</p>
</template>
