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