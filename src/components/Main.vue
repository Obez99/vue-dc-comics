<template>
  <main>
    <div class="jumbotron"></div>
    <h4>CURRENT SERIES</h4>
    <div class="products-container">
      <Product
        v-for="(product, i) in products"
        :key="i"
        :thumb="product.thumb"
        :series="product.series"
      ></Product>
      <button>LOAD MORE</button>
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
  background-color: rgb(28, 28, 28);
  h4 {
    background-color: $primary-color;
    display: inline-block;
    padding: 10px 25px;
    margin: 0;
    margin-left: $sections-padding-horizontal - 15px;
    transform: translateY(-27px);
  }

  button {
    background-color: $primary-color;
    padding: 10px 50px;
    color: white;
    border: none;
    cursor: pointer;
    margin: auto;
  }

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