<template>
  <section id="main-menu">
    <div class="container">
      <ul>
        <li>
          <a href="">
            <img
              src="../../assets/img/buy-comics-digital-comics.png"
              alt="digital comics icon"
            />
            Digital comics
          </a>
        </li>
        <li>
          <a href="">
            <img
              src="../../assets/img/buy-comics-merchandise.png"
              alt="dc merchandise icon"
            />
            Dc merchandise
          </a>
        </li>
        <li>
          <a href="">
            <img
              src="../../assets/img/buy-comics-subscriptions.png"
              alt="subscription icon"
            />
            Subscription
          </a>
        </li>
        <li>
          <a href="">
            <img
              src="../../assets/img/buy-comics-shop-locator.png"
              alt="Comic shop locator icon"
            />
            Comic shop locator
          </a>
        </li>
        <li>
          <a href="">
            <img
              src="../../assets/img/buy-dc-power-visa.svg"
              alt="Dc power visa icon"
            />
            Dc power visa
          </a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainMenu",
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/partials/_variables.scss";
#main-menu {
  padding: 2rem 0;
  text-align: center;
  background-color: $brandColor;
}
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
</style>
