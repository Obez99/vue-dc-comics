<template>
  <main>
    <div class="jumbotron"></div>
    <div class="products-container">
      <div class="box">CURRENT SERIES</div>
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
    padding: 0 $sections-padding-horizontal;

    .box {
      font-size: 25px;
      display: inline-block;
      padding: 15px 20px;
      background-color: $primary-color;
      transform: translateY(-29.5px);
    }
  }
}
</style>