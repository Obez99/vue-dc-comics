<template>
  <div class="bottom-footer">
    <div>
      <button>SIGN-UP NOW!</button>
    </div>

    <div class="social-section">
      <h3>FOLLOW US</h3>

      <ul>
        <li v-for="(listItem, i) in socialButtons" :key="i">
          <a href="#"
            ><img
              :src="require('../assets/' + listItem.image)"
              :alt="listItem.name"
          /></a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "BottomFooter",
  data() {
    return {
      socialButtons: [
        {
          name: "Facebook",
          image: "footer-facebook.png",
        },
        {
          name: "Twitter",
          image: "footer-twitter.png",
        },
        {
          name: "Youtube",
          image: "footer-youtube.png",
        },
        {
          name: "Pinterest",
          image: "footer-pinterest.png",
        },
        {
          name: "Periscope",
          image: "footer-periscope.png",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../styles/variables";

.bottom-footer {
  z-index: 1;
  background-color: rgb(48, 48, 48);

  display: flex;
  justify-content: space-between;
  align-items: center;

  button {
    background: none;
    border: 1px solid $primary-color;
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
      color: $primary-color;
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