<template>
  <main>
    <div class="jumbotron"></div>
    <div class="products-container">
      <div v-for="(product, i) in products" :key="i" class="product">
        <div class="product-image">
          <img :src="product.thumb" :alt="product.series" />
        </div>
        <h5>{{ product.series }}</h5>
      </div>
    </div>
  </main>
</template>

<script>
import products from "../assets/dc-comics.json";

export default {
  name: "Main",
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

    .product {
      width: calc(100% / 6 - 30px);

      .product-image {
        height: 250px;

        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: top;
        }
      }

      h5 {
        margin: 0;
      }
    }
  }
}
</style>