<template>
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
</template>

<script>
export default {
  name: "MiddleFooter",
};
</script>

<style scoped lang="scss">
.middle-footer {
  background-image: url("../assets/footer-bg.jpg");
  background-size: cover;
  overflow: hidden;
  padding: 40px 0;
  display: flex;
  justify-content: space-between;

  .left-middle-footer {
    display: flex;

    ul {
      list-style: none;
      display: inline-block;
      padding-inline-start: 0;

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