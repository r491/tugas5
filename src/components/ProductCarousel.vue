<!-- ProductCarousel.vue -->
<template>
  <div class="product-carousel">
    <div class="carousel-item">
      <div class="product-card">
        <img src="/th.jpeg" alt="Product 1">
        <!-- Product content -->
      </div>
    </div>
    <!-- Add more carousel items -->
  </div>
</template>

<style>
.product-carousel {
  display: flex;
  justify-content: center;
}

.carousel-item {
  margin: 0 10px; /* Jarak antara setiap item carousel */
}

.product-card {
  width: 300px; /* Atur lebar card sesuai kebutuhan */
  height: 400px; /* Atur tinggi card sesuai kebutuhan */
  border: 1px solid #ccc;
  border-radius: 5px;
  overflow: hidden;
  margin: 0 auto; /* Mengatur margin auto untuk membuatnya berada di tengah */
}

.product-card img {
  width: 100%; /* Mengatur gambar agar terisi sepenuhnya dalam card */
  height: auto; /* Menjaga aspek rasio gambar */
}
</style>
