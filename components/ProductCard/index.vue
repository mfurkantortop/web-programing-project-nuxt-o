<template>
    <div class="border rounded-lg shadow-md p-4">
      <img :src="image" alt="Product Image" class="w-full h-40 object-cover rounded-md mb-4" />
      <h3 class="text-lg font-semibold mb-2">{{ title }}</h3>
      <p class="text-gray-700 mb-2">{{ description }}</p>
      <span class="text-green-600 font-bold">{{ price }}</span>
    </div>
  </template>
  
  <script lang="ts" setup>
  defineProps({
    image: String,
    title: String,
    description: String,
    price: String,
  });
  </script>
  
  <style scoped>
  </style>
  