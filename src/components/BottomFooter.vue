<template>
  <div class="bottom-footer">
    <div>
      <button>SIGN-UP NOW!</button>
    </div>

    <div class="social-section">
      <h3>FOLLOW US</h3>

      <ul>
        <li>
          <a href="#"
            ><img src="../assets/footer-facebook.png" alt="dc-facebook"
          /></a>
        </li>
        <li>
          <a href="#"
            ><img src="../assets/footer-twitter.png" alt="dc-twitter"
          /></a>
        </li>
        <li>
          <a href="#"
            ><img src="../assets/footer-youtube.png" alt="dc-youtube"
          /></a>
        </li>
        <li>
          <a href="#"
            ><img src="../assets/footer-pinterest.png" alt="dc-pinteres"
          /></a>
        </li>
        <li>
          <a href="#"
            ><img src="../assets/footer-periscope.png" alt="dc-periscope"
          /></a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "BottomFooter",
};
</script>

<style scoped lang="scss">
.bottom-footer {
  z-index: 1;
  background-color: rgb(48, 48, 48);

  display: flex;
  justify-content: space-between;
  align-items: center;

  button {
    background: none;
    border: 1px solid #0282f9;
    color: white;
    padding: 15px;
    cursor: pointer;
    font-size: 15px;
    font-weight: bold;
  }

  .social-section {
    display: flex;
    align-items: center;

    h3 {
      color: #0282f9;
    }

    ul {
      list-style: none;
    }

    li {
      display: inline-block;
      margin-left: 20px;
    }

    img {
      width: 40px;
    }
  }
}
</style>