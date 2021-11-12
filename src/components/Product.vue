<template>
  <div class="product">
    <div class="product-image">
      <img :src="thumb" :alt="series" />
    </div>
    <h5>{{ series }}</h5>
  </div>
</template>

<script>
export default {
  name: "Product",
  props: {
    thumb: String,
    series: String,
  },
};
</script>

<style scoped lang="scss">
.product {
  width: calc(100% / 6 - 30px);

  .product-image {
    height: 250px;
    margin-bottom: 20px;

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
</style>