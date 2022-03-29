<template>
  <section id="main-menu">
    <div class="container">
      <ul>
        <li v-for="(item, index) in menuItems" :key="index">
          <a href="">
            <img
              :src="require(`../../assets/img/${item.src}`)"
              :alt="item.alt"
            />
            <h4 class="text-uppercase">{{ item.text }}</h4>
          </a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainMenu",
  data() {
    return {
      menuItems: [
        {
          src: "buy-comics-digital-comics.png",
          alt: "digital comics image",
          text: "Digital Comics",
        },
        {
          src: "buy-comics-merchandise.png",
          alt: "comics merchandise image",
          text: "Dc merchandise",
        },
        {
          src: "buy-comics-subscriptions.png",
          alt: "comics subscriptions image",
          text: "Subscription",
        },
        {
          src: "buy-comics-shop-locator.png",
          alt: "comics shop locator image",
          text: "Comic shop locator",
        },
        {
          src: "buy-dc-power-visa.svg",
          alt: "dc power visa image",
          text: "Dc power visa",
        },
      ],
    };
  },
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
  @include flex(center, center, row, 4rem);
  li {
    padding: 0.7rem;
    font-size: 1rem;
    display: inline-block;
    a {
      @include flex(center, center, row, 0);
      color: white;
      img {
        height: 60px;
        max-width: 60px;
        margin-right: 0.8rem;
      }
      h4 {
        font-weight: 400;
      }
    }
  }
}
</style>
