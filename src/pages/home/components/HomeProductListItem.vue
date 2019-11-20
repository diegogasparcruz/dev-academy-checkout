<template>
  <div class="product-list-item">
    <h3>{{ product.id }}</h3>
  </div>
</template>

<script>
export default {
  name: "HomeProductListItem",
  props: {
    product: Object
  }
};
</script>