<template>
    <section>
      <h2 class="text-2xl font-bold mb-4">Featured Products</h2>
      <div class="grid grid-cols-2 gap-4">
        <ProductCard
          v-for="product in products"
          :key="product.id"
          :image="product.image"
          :title="product.title"
          :description="product.description"
          :price="product.price"
        />
      </div>
    </section>
  </template>
  
  <script lang="ts" setup>
  import ProductCard from '~/components/ProductCard/index.vue';
  
  defineProps({
    products: Array as () => {
      id: number;
      image: string;
      title: string;
      description: string;
      price: string;
    }[],
  });
  </script>
  
  <style scoped>
  </style>
  