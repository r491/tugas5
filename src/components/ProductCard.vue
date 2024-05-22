<template>
  <div class="product-card">
    <img :src="product.image" alt="Product Image">
    <div class="product-info">
      <h3>{{ product.name }}</h3>
      <p>{{ product.description }}</p>
      <p>Price: ${{ product.price }}</p>
      <button>Add to Cart</button>
    </div>
  </div>
</template>

<script>
export default {
  // Logic for ProductCard component
  props: ['product']
}
</script>

<style>
.product-card {
  width: 300px;
  margin: 0 auto; /* Mengatur margin auto untuk membuatnya berada di tengah */
  border: 1px solid #ccc;
  border-radius: 5px;
  overflow: hidden;
}

.product-card img {
  width: 100%;
  height: auto;
}

.product-info {
  padding: 10px;
}

.product-info h3 {
  margin-top: 0;
}

.product-info p {
  margin: 5px 0;
}

.product-info button {
  background-color: #333;
  color: #fff;
  padding: 5px 10px;
  border: none;
  border-radius: 3px;
  cursor: pointer;
}

.product-info button:hover {
  background-color: #555;
}
</style>
