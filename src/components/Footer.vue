<template>
  <footer class="home-footer">
    <section class="footer-nav">
      <div class="container">
        <nav>
          <div class="footer-list-col">
            <h4>Dc Comics</h4>
            <ul>
              <li v-for="(link, index) in footerDcComicsNavLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
            <h4>Shop</h4>
            <ul>
              <li v-for="(link, index) in footerShopNavLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="footer-list-col">
            <h4>Dc</h4>
            <ul>
              <li v-for="(link, index) in footerDcNavLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="footer-list-col">
            <h4>Sites</h4>
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
        <button>Sign up now!</button>
        <div class="socials">
          <h4>Follow us</h4>
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
          text: "Collectibles",
          active: false,
          url: "#",
        },
        {
          text: "Videos",
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
      @include flex(flex-start, flex-start, row, 2rem);
      background: url("../assets/img/dc-logo-bg.png") no-repeat right;
      div.footer-list-col {
        padding-bottom: 3.5rem;
        h4 {
          margin-bottom: 0.5rem;
          text-transform: uppercase;
        }
        a {
          font-size: 0.85rem;
          color: rgb(156, 156, 156);
        }
      }
    }
  }
  section.footer-social {
    padding: 1rem 0;
    background-color: #303030;
    div.container {
      @include flex(center, space-between, row, 0);
      button {
        background-color: transparent;
        color: white;
        font-size: 1rem;
        text-transform: uppercase;
        height: 50px;
        padding: 0 1rem;
        border: 2px solid $brandColor;
      }
      div.socials {
        @include flex(center, space-between, row, 1.5rem);
        h4 {
          color: $brandColor;
          text-transform: uppercase;
        }
        img {
          width: 35px;
        }
      }
    }
  }
}
</style>
