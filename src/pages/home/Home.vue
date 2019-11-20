<template>
  <div class="home">
    <h1>Qualquer coisa</h1>
    <HomeProductList class="product-list" />
    <HomePaymentSummary class="payment-summary" />
  </div>
</template>

<script>
import HomeProductList from "./components/HomeProductList";
import HomePaymentSummary from "./components/HomePaymentSummary";

export default {
  name: "home",
  components: {
    HomeProductList,
    HomePaymentSummary
  }
};
</script>

<style lang="stylus">
.home {
  width: 100%;
}

@media screen and (min-width: 950px) {
  .home {
    display: flex;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .product-list {
    margin-right: 2%;
  }
}

@media screen and (min-width: 1300px) {
  .home {
    display: flex;
    width: 70%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}
</style>
