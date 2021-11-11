<template>
  <header>
    <img src="../assets/dc-logo.png" alt="header-logo" />

    <nav>
      <ul>
        <li><a href="#">CHARACTERS</a></li>
        <li><a href="#">COMICS</a></li>
        <li><a href="#">MOVIES</a></li>
        <li><a href="#">TV</a></li>
        <li><a href="#">GAMES</a></li>
        <li><a href="#">COLLECTIBLES</a></li>
        <li><a href="#">VIDEOS</a></li>
        <li><a href="#">FANS</a></li>
        <li><a href="#">NEWS</a></li>
        <li><a href="#">SHOP</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped lang="scss">
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 0;

  ul {
    list-style: none;
    font-weight: bold;

    li {
      display: inline-block;

      a {
        text-decoration: none;
        color: inherit;
        display: inline-block;

        padding: 10px 20px;
      }

      &:hover {
        color: #0282f9;
      }
    }
  }

  img {
    width: 100px;
    height: 100px;
  }
}
</style>