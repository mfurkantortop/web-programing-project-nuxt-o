<template>
    <div>
      <Header />
      <ProfileHeader />
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

