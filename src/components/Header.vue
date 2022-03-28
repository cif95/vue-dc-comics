<template>
  <div class="home-header">
    <div class="container">
      <div class="header-logo">
        <img src="../assets/img/dc-logo.png" alt="dc comics logo" />
      </div>
      <nav>
        <ul>
          <li
            :class="{ active: link.active }"
            v-for="(link, index) in headerNavLinks"
            :key="index"
          >
            <a :href="link.url">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeHeader",
  data: function () {
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
};
</script>

<style scoped lang="scss">
div.container {
  width: 70%;
  display: flex;
  margin: 0 auto;
  align-items: center;
  justify-content: space-between;
  img {
    padding-top: 0.5rem;
    width: 80px;
  }
  ul {
    margin: 0;
    li {
      list-style-type: none;
      display: inline-block;
      margin-right: 1.2rem;
      padding: 3rem 0;
      font-size: 0.85rem;
      font-weight: 600;
      text-transform: uppercase;
      border-bottom: 5px solid transparent;
      &.active {
        border-color: #107eec;
        a {
          color: #107eec;
        }
      }
      a {
        color: rgb(51, 51, 51);
        text-decoration: none;
      }
    }
  }
}
</style>
