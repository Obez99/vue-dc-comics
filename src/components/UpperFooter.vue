<template>
  <div class="upper-footer">
    <ul>
      <li v-for="(item, i) in shopItems" :key="i">
        <a href="#"
          ><img :src="item.image" :alt="item.text" />{{ item.text }}</a
        >
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "UpperFooter",
  data() {
    return {
      shopItems: [
        {
          image: "../assets/buy-comics-digital-comics.png",
          text: "DIGITAL COMICS",
        },
        {
          image: "../assets/buy-comics-merchandise.png",
          text: "DC MERCHANDISE",
        },
        {
          image: "../assets/buy-comics-subscriptions.png",
          text: "SUBSCRIPTION",
        },
        {
          image: "../assets/buy-comics-shop-locator.png",
          text: "COMIC SHOP LOCATOR",
        },
        {
          image: "../assets/buy-dc-power-visa.png",
          text: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.upper-footer {
  background-color: #0282f9;
  padding: 50px 0;

  img {
    width: 50px;
    height: 60px;
    margin-right: 10px;
  }

  ul {
    list-style: none;

    display: flex;
    justify-content: space-around;
    align-items: center;

    a {
      color: white;
      text-decoration: none;

      display: flex;
      align-items: center;
    }
  }
}
</style>