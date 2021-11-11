<template>
  <div class="upper-footer">
    <ul>
      <li>
        <a href="#"
          ><img src="../assets/buy-comics-digital-comics.png" alt="" />DIGITAL
          COMICS</a
        >
      </li>
      <li>
        <a href="#"
          ><img src="../assets/buy-comics-merchandise.png" alt="" />DC
          MERCHANDISE</a
        >
      </li>
      <li>
        <a href="#"
          ><img
            src="../assets/buy-comics-subscriptions.png"
            alt=""
          />SUBSCRIPTION</a
        >
      </li>
      <li>
        <a href="#"
          ><img src="../assets/buy-comics-shop-locator.png" alt="" />COMIC SHOP
          LOCATOR</a
        >
      </li>
      <li>
        <a href="#"
          ><img src="../assets/buy-dc-power-visa.svg" alt="" />DC POWER VISA</a
        >
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "UpperFooter",
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