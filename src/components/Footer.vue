<template>
  <div class="home-footer">
    <div class="footer-nav">
      <div class="container">
        <nav>
          <div class="footer-list">
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
          <div class="footer-list">
            <h4>Dc</h4>
            <ul>
              <li v-for="(link, index) in footerDcNavLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="footer-list">
            <h4>Sites</h4>
            <ul>
              <li v-for="(link, index) in footerSitesNavLinks" :key="index">
                <a :href="link.url">{{ link.text }}</a>
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </div>
    <div class="footer-social">
      <div class="container">
        <button>Sign up now!</button>
        <div class="socials">
          <h4>Follow us</h4>
          <img src="../assets/img/footer-facebook.png" alt="facebook logo" />
          <img src="../assets/img/footer-twitter.png" alt="twitter logo" />
          <img src="../assets/img/footer-youtube.png" alt="youtube logo" />
          <img src="../assets/img/footer-pinterest.png" alt="pinterest logo" />
          <img src="../assets/img/footer-periscope.png" alt="periscope logo" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeFooter",
  data: function () {
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
    };
  },
};
</script>

<style scoped lang="scss">
div.container {
  width: 70%;
  color: white;
  padding: 1rem 0;
  margin: 0 auto;
}
div.home-footer {
  div.footer-nav {
    background-image: url(../assets/img/footer-bg.jpg);
    nav {
      display: flex;
      gap: 2rem;
      div.footer-list {
        h4 {
          margin-bottom: 0.5rem;
          text-transform: uppercase;
        }
        ul {
          margin-top: 0;
          padding-left: 0;
          li {
            list-style-type: none;
            a {
              font-size: 0.75rem;
              color: rgb(156, 156, 156);
              text-decoration: none;
            }
          }
        }
      }
    }
  }
  div.footer-social {
    padding: 2rem;
    background-color: #232323;
    div.container {
      display: flex;
      justify-content: space-between;
      button {
        background-color: transparent;
        color: white;
        font-weight: 600;
        font-size: 1rem;
        text-transform: uppercase;
        height: 50px;
        padding: 0 1rem;
        border: 2px solid #107eec;
      }
      div.socials {
        display: flex;
        gap: 1rem;
        align-items: center;
        h4 {
          color: #107eec;
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
