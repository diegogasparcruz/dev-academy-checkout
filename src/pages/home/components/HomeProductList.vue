<template>
  <div class="home-product-list">
    <h2 class="title">Produtos</h2>
    <div class="product-list-container">
      <HomeProductListItem v-for="product in products" :key="product.id" />
    </div>
  </div>
</template>

<script>
import HomeProductListItem from "./HomeProductListItem";

export default {
  name: "HomeProductList",
  components: {
    HomeProductListItem
  }
};
</script>