<template>
  <footer class="home-footer">
    <section class="footer-nav">
      <div class="container">
        <nav>
          <div class="footer-list-col">
            <h3 class="text-uppercase">Dc Comics</h3>
            <ul>
              <li v-for="(link, index) in footerDcComicsNavLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
            <h3 class="text-uppercase">Shop</h3>
            <ul>
              <li v-for="(link, index) in footerShopNavLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="footer-list-col">
            <h3 class="text-uppercase">Dc</h3>
            <ul>
              <li v-for="(link, index) in footerDcNavLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="footer-list-col">
            <h3 class="text-uppercase">Sites</h3>
            <ul>
              <li v-for="(link, index) in footerSitesNavLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </section>
    <section class="footer-social">
      <div class="container">
        <button class="my-btn-outline-primary">Sign up now!</button>
        <div class="socials">
          <h2 class="text-uppercase">Follow us</h2>
          <img
            v-for="(item, index) in footerSocials"
            :key="index"
            :src="require(`../assets/img/${item.src}`)"
            :alt="item.alt"
          />
        </div>
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: "HomeFooter",
  data() {
    return {
      footerDcComicsNavLinks: [
        {
          text: "Characters",
          active: false,
          url: "#",
        },
        {
          text: "Comics",
          active: true,
          url: "#",
        },
        {
          text: "Movies",
          active: false,
          url: "#",
        },
        {
          text: "Tv",
          active: false,
          url: "#",
        },
        {
          text: "Games",
          active: false,
          url: "#",
        },
        {
          text: "Videos",
          active: false,
          url: "#",
        },
        {
          text: "News",
          active: false,
          url: "#",
        },
      ],
      footerShopNavLinks: [
        {
          text: "Shop DC",
          active: false,
          url: "#",
        },
        {
          text: "Shop DC collectible",
          active: true,
          url: "#",
        },
      ],
      footerDcNavLinks: [
        {
          text: "Terms of Use",
          active: false,
          url: "#",
        },
        {
          text: "Privacy policy(New)",
          active: true,
          url: "#",
        },
        {
          text: "Ad choices",
          active: false,
          url: "#",
        },
        {
          text: "Advertising",
          active: false,
          url: "#",
        },
        {
          text: "Jobs",
          active: false,
          url: "#",
        },
        {
          text: "Subscriptions",
          active: false,
          url: "#",
        },
        {
          text: "Talent workshops",
          active: false,
          url: "#",
        },
        {
          text: "CPSC Certificates",
          active: false,
          url: "#",
        },
        {
          text: "Ratings",
          active: false,
          url: "#",
        },
        {
          text: "Shop Help",
          active: false,
          url: "#",
        },
        {
          text: "Contact Us",
          active: false,
          url: "#",
        },
      ],
      footerSitesNavLinks: [
        {
          text: "DC",
          active: false,
          url: "#",
        },
        {
          text: "MAD Magazine",
          active: true,
          url: "#",
        },
        {
          text: "DC Kids",
          active: false,
          url: "#",
        },
        {
          text: "DC Universe",
          active: false,
          url: "#",
        },
        {
          text: "DC Power Visa",
          active: false,
          url: "#",
        },
      ],
      footerSocials: [
        {
          src: "footer-facebook.png",
          alt: "facebook logo",
        },
        {
          src: "footer-twitter.png",
          alt: "twitter logo",
        },
        {
          src: "footer-youtube.png",
          alt: "youtube logo",
        },
        {
          src: "footer-pinterest.png",
          alt: "pinterest logo",
        },
        {
          src: "footer-periscope.png",
          alt: "periscope logo",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/partials/_variables.scss";
footer.home-footer {
  section.footer-nav {
    background-image: url(../assets/img/footer-bg.jpg);
    nav {
      padding-top: 1rem;
      @include flex(flex-start, flex-start, row, 2rem);
      background: url("../assets/img/dc-logo-bg.png") no-repeat right;
      div.footer-list-col {
        padding-bottom: 3.5rem;
        h3 {
          margin-bottom: 0.5rem;
        }
        li {
          padding: 0.12rem 0;
          a {
            font-size: 0.8rem;
            color: rgb(156, 156, 156);
          }
        }
      }
    }
  }
  section.footer-social {
    padding: 1rem 0;
    background-color: #303030;
    font-family: "Asap Condensed", sans-serif;
    div.container {
      @include flex(center, space-between, row, 0);
      div.socials {
        @include flex(center, space-between, row, 1.5rem);
        h2 {
          color: $brandColor;
        }
        img {
          width: 35px;
        }
      }
    }
  }
}
</style>
