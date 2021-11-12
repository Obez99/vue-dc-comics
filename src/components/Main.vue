<template>
  <main>
    <div class="jumbotron"></div>
    <div class="products-container">
      <Product
        v-for="(product, i) in products"
        :key="i"
        :thumb="product.thumb"
        :series="product.series"
      ></Product>
    </div>
  </main>
</template>

<script>
import products from "../assets/dc-comics.json";
import Product from "./Product.vue";
export default {
  name: "Main",
  components: { Product },
  data() {
    return {
      products: products,
    };
  },
};
</script>

<style scoped lang="scss">
@import "../styles/variables";

main {
  font-size: 30px;
  color: white;
  background-color: black;

  .jumbotron {
    width: 100%;
    height: 400px;
    background-image: url("../assets/jumbotron.jpg");
  }

  .products-container {
    padding: $sections-padding-vertical $sections-padding-horizontal;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 30px;
  }
}
</style>