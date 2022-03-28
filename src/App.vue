<template>
  <div id="app">
    <Header />
    <main>
      <div class="content">
        <div class="container">
          <h3>Content goes here</h3>
        </div>
      </div>
      <div class="banner">
        <div class="container">
          <ul>
            <li>
              <a href="">
                <img
                  src="./assets/img/buy-comics-digital-comics.png"
                  alt="digital comics icon"
                />
                Digital comics
              </a>
            </li>
            <li>
              <a href="">
                <img
                  src="./assets/img/buy-comics-merchandise.png"
                  alt="dc merchandise icon"
                />
                Dc merchandise
              </a>
            </li>
            <li>
              <a href="">
                <img
                  src="./assets/img/buy-comics-subscriptions.png"
                  alt="subscription icon"
                />
                Subscription
              </a>
            </li>
            <li>
              <a href="">
                <img
                  src="./assets/img/buy-comics-shop-locator.png"
                  alt="Comic shop locator icon"
                />
                Comic shop locator
              </a>
            </li>
            <li>
              <a href="">
                <img
                  src="./assets/img/buy-dc-power-visa.svg"
                  alt="Dc power visa icon"
                />
                Dc power visa
              </a>
            </li>
          </ul>
        </div>
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
@import "./assets/scss/style.scss";
#app {
  font-family: "Asap Condensed", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 140%;
}
div.container {
  color: white;
}
div.content {
  padding: 1rem;
  background-color: black;
}
div.banner {
  padding: 2rem 0;
  text-align: center;
  background-color: #0282f9;
  ul {
    display: flex;
    justify-content: space-around;
    li {
      padding: 0.7rem;
      text-transform: uppercase;
      font-size: 1rem;
      display: inline-block;
      a {
        color: white;
        img {
          height: 50px;
          max-width: 50px;
          margin-right: 0.8rem;
          vertical-align: middle;
        }
      }
    }
  }
}
</style>
