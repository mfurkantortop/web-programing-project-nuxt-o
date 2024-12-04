<template>
    <ul class="flex gap-4">
      <li v-for="category in categories" :key="category" class="bg-gray-100 p-2 rounded-md shadow">
        {{ category }}
      </li>
    </ul>
  </template>
  
  <script lang="ts" setup>
  defineProps({
    categories: Array as () => string[],
  });
  </script>
  
  <style scoped>
  </style>
  