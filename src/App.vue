<template>
  <div id="app">
    <Header />
    <main>
      <div class="container">
        <h3>Content goes here</h3>
      </div>
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Asap+Condensed:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600&display=swap");
#app {
  font-family: "Asap Condensed", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 140%;
}
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  main {
    color: white;
    padding: 3rem;
    background-color: black;
    div.container {
      width: 70%;
      color: white;
      padding: 1rem 0;
      margin: 0 auto;
    }
  }
}
</style>
