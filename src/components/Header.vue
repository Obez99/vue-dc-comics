<template>
  <header>
    <img src="../assets/dc-logo.png" alt="header-logo" />

    <nav>
      <ul>
        <li v-for="(item, i) in navItems" :key="i">
          <a href="#">{{ item }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      navItems: [
        "CHARACTERS",
        "COMICS",
        "MOVIES",
        "TV",
        "GAMES",
        "COLLECTIBLES",
        "VIDEOS",
        "FANS",
        "NEWS",
        "SHOP",
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../styles/variables";

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: $sections-padding-vertical $sections-padding-horizontal;
  ul {
    list-style: none;
    font-weight: bold;

    li {
      display: inline-block;

      a {
        text-decoration: none;
        color: inherit;
        display: inline-block;
        padding: $sections-padding-vertical;
      }

      &:hover {
        color: $primary-color;
      }
    }
  }

  img {
    width: 100px;
    height: 100px;
  }
}
</style>