<template>
  <div id="app">
    <Header />
    <Content />
    <Footer />
  </div>
</template>

<script>
import Header from "./layouts/Header";
import Content from "./layouts/Content";
import Footer from "./layouts/Footer";

export default {
  name: "App",
  components: {
    Header,
    Content,
    Footer,
  },
};
</script>

<style>
body {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

  height: 100vh;
  display: grid;
  grid-template-rows: 4em 1fr 6em;
  grid-auto-columns: ifr;
  grid-template-areas: "header" "content" "footer";
}
</style>
