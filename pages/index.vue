<template>
    <div>
      <Header />
      <HeroSection />
      <SearchBar />
      <FeaturedProducts :products="products" />
      <CategoryList :categories="categories" />
      <Testimonial
        message=""
        name=""
      />
      <NewsletterSignup />
      <Footer />
    </div>
  </template>

<script lang="ts" setup>
import Header from '@/components/Header.vue';
import HeroSection from '@/components/HeroSection.vue';
import SearchBar from '@/components/SearchBar.vue';
import FeaturedProducts from '@/components/FeaturedProducts.vue';
import CategoryList from '@/components/CategoryList.vue';
import Testimonial from '@/components/Testimonial.vue';
import NewsletterSignup from '@/components/NewsletterSignup.vue';
import Footer from '@/components/Footer.vue';

const products = [
  {
    id: 1,
    image: '/product1.jpg',
    title: 'Product 1',
    description: 'Amazing product',
    price: '$29.99',
  },
  {
    id: 2,
    image: '/product2.jpg',
    title: 'Product 2',
    description: 'Great value',
    price: '$39.99',
  },
];

const categories = ['Clothing', 'Accessories', 'Shoes', 'Sale'];
</script>

<style scoped>
</style>