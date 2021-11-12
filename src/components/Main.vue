<template>
  <main>
    <div class="jumbotron"></div>
    <div class="products-container">
      <div class="product">
        <img src="../assets/buy-comics-digital-comics.png" alt="" />
        <h5>ACTION COMICS</h5>
      </div>
      <div class="product">
        <img src="../assets/buy-comics-digital-comics.png" alt="" />
        <h5>ACTION COMICS</h5>
      </div>
      <div class="product">
        <img src="../assets/buy-comics-digital-comics.png" alt="" />
        <h5>ACTION COMICS</h5>
      </div>
      <div class="product">
        <img src="../assets/buy-comics-digital-comics.png" alt="" />
        <h5>ACTION COMICS</h5>
      </div>
      <div class="product">
        <img src="../assets/buy-comics-digital-comics.png" alt="" />
        <h5>ACTION COMICS</h5>
      </div>
      <div class="product">
        <img src="../assets/buy-comics-digital-comics.png" alt="" />
        <h5>ACTION COMICS</h5>
      </div>
      <div class="product">
        <img src="../assets/buy-comics-digital-comics.png" alt="" />
        <h5>ACTION COMICS</h5>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "Main",
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

      img {
        width: 100%;
      }
    }
  }
}
</style>