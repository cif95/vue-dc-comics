<template>
  <div>
    <MainJumbo />
    <MainContent />
    <MainMenu />
  </div>
</template>

<script>
import MainJumbo from "./MainJumbo.vue";
import MainContent from "./MainContent.vue";
import MainMenu from "./MainMenu.vue";

export default {
  name: "HomeMain",
  components: {
    MainJumbo,
    MainContent,
    MainMenu,
  },
};
</script>

<style lang="scss">
@import "../../assets/scss/partials/_variables.scss";

div.container {
  color: white;
}
</style>
