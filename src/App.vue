<template>
  <div id="app">
    <Header></Header>
    <Main></Main>
    <footer>
      <UpperFooter></UpperFooter>
      <MiddleFooter></MiddleFooter>
      <BottomFooter></BottomFooter>
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import UpperFooter from "./components/UpperFooter.vue";
import MiddleFooter from "./components/MiddleFooter.vue";
import BottomFooter from "./components/BottomFooter.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    UpperFooter,
    MiddleFooter,
    BottomFooter,
  },
};
</script>

<style lang="scss">
body {
  margin: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
