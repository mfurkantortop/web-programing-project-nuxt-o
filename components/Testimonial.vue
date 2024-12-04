<template>
    <div class="border p-4 rounded-lg shadow-md">
      <p class="italic">"{{ message }}"</p>
      <p class="text-right font-semibold">- {{ name }}</p>
    </div>
  </template>
  
  <script lang="ts" setup>
  defineProps({
    message: String,
    name: String,
  });
  </script>
  
  <style scoped>
  </style>
  