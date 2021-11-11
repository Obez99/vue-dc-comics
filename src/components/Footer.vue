<template>
  <footer>
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
            ><img src="../assets/buy-comics-shop-locator.png" alt="" />COMIC
            SHOP LOCATOR</a
          >
        </li>
        <li>
          <a href="#"
            ><img src="../assets/buy-dc-power-visa.svg" alt="" />DC POWER
            VISA</a
          >
        </li>
      </ul>
    </div>

    <div class="middle-footer">
      <div class="left-middle-footer">
        <ul>
          <h3>DC COMICS</h3>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>

          <h3>SHOP</h3>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>

        <ul>
          <h3>DC</h3>
          <li><a href="#">Terms of Use</a></li>
          <li><a href="#">Privacy Policy (New)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Rating</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>

        <ul>
          <h3>SITES</h3>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>

      <div class="right-middle-footer">
        <img src="../assets/dc-logo-bg.png" alt="" />
      </div>
    </div>

    <div class="bottom-footer"></div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
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

.middle-footer {
  background-image: url("../assets/footer-bg.jpg");
  background-size: cover;
  padding: 40px 0;
  display: flex;
  justify-content: space-between;

  .left-middle-footer {
    display: flex;

    ul {
      list-style: none;
      display: inline-block;

      li {
        margin-bottom: 5px;
      }
      a {
        color: gray;
        text-decoration: none;
      }
    }

    h3 {
      color: white;
    }
  }

  .right-middle-footer {
    position: relative;
    img {
      width: 600px;
      position: absolute;
      right: 0;
      top: -100px;
    }
  }
}
</style>