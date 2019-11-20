<template>
  <div class="home">
    <h1>Qualquer coisa</h1>
    <HomeProductList />
  </div>
</template>

<script>
import HomeProductList from "./components/HomeProductList";

export default {
  name: "home",
  components: {
    HomeProductList
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
