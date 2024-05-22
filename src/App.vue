<template>
  <div id="app">
    <page-navbar></page-navbar>
    <product-carousel></product-carousel>
    <div class="container">
      <product-card v-for="product in products" :key="product.id" :product="product"></product-card>
    </div>
    <page-footer></page-footer>
  </div>
</template>

<script>
import PageNavbar from './components/PageNavbar.vue';
import ProductCarousel from './components/ProductCarousel.vue';
import ProductCard from './components/ProductCard.vue';
import PageFooter from './components/PageFooter.vue';

export default {
  components: {
    PageNavbar,
    ProductCarousel,
    ProductCard,
    PageFooter
  },
  data() {
    return {
      products: [
        {
          id: 1,
          name: "Product 1",
          description: "Description of Product 1",
          price: 10,
          image: "/th (1).jpeg"
        },
        {
          id: 2,
          name: "Product 2",
          description: "Description of Product 2",
          price: 20,
          image: "./th (2).jpeg"
        },
        // Add more products as needed
      ]
    };
  }
}
</script>

<style>
/* Styles for App.vue */
</style>
