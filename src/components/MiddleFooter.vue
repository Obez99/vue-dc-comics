<template>
  <div class="middle-footer">
    <div class="left-middle-footer">
      <ul
        v-for="(list, i) in footerList"
        :key="i"
        :class="list.title === 'SHOP' ? 'shop-list' : ''"
      >
        <h3>{{ list.title }}</h3>
        <li v-for="(listItem, i) in list.listItems" :key="i">
          <a href="#">{{ listItem }}</a>
        </li>
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
  data() {
    return {
      footerList: [
        {
          title: "DC COMICS",
          listItems: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Videos",
            "News",
          ],
        },
        {
          title: "SHOP",
          listItems: ["Shop DC", "Shop DC Collectibles"],
        },
        {
          title: "DC",
          listItems: [
            "Terms of Use",
            "Privacy policy (New)",
            "Ad Choices",
            "Advertising",
            "Jobs",
            "Subscriptions",
            "Talent Worksops",
            "CPSC Certificates",
            "Ratings",
            "Shop Help",
            "Contact Us",
          ],
        },
        {
          title: "SITES",
          listItems: [
            "DC",
            "MAD Magazine",
            "DC Kids",
            "DC Universe",
            "DC Power Visa",
          ],
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../styles/variables";

.middle-footer {
  background-image: url("../assets/footer-bg.jpg");
  background-size: cover;
  overflow: hidden;
  padding: $sections-padding-vertical $sections-padding-horizontal;
  display: flex;
  justify-content: space-between;

  .left-middle-footer {
    display: flex;
    position: relative;

    .shop-list {
      position: absolute;
      bottom: 0;
      left: 0;
    }

    ul {
      list-style: none;
      display: inline-block;
      padding-inline-start: 0;
      margin-right: 80px;
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