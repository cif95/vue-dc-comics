<template>
  <header class="home-header">
    <div class="container">
      <div class="header-logo">
        <img src="../assets/img/dc-logo.png" alt="dc comics logo" />
      </div>
      <nav class="header-nav">
        <ul>
          <li
            :class="{ active: link.active }"
            v-for="(link, index) in headerNavLinks"
            :key="index"
            @click="updateCurrentActive(index)"
          >
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "HomeHeader",
  data() {
    return {
      headerNavLinks: [
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
        {
          text: "Fans",
          active: false,
          url: "#",
        },
        {
          text: "News",
          active: false,
          url: "#",
        },
        {
          text: "Shop",
          active: false,
          url: "#",
        },
      ],
    };
  },
  methods: {
    updateCurrentActive(currentIndex) {
      this.headerNavLinks.forEach((link, index) => {
        if (currentIndex === index) {
          link.active = true;
        } else {
          link.active = false;
        }
      });
    },
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/partials/_variables.scss";
div.container {
  @include flex(center, space-between, row, 0);
  img {
    padding-top: 0.5rem;
    width: 80px;
  }
  li {
    padding: 3rem 0;
    font-weight: 600;
    margin-right: 2rem;
    font-size: 0.85rem;
    display: inline-block;
    text-transform: uppercase;
    border-bottom: 5px solid transparent;
    &.active {
      border-color: $brandColor;
      a {
        color: $brandColor;
      }
    }
    a {
      color: rgb(70, 70, 70);
    }
  }
}
</style>
