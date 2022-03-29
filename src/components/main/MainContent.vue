<template>
  <section class="main-content">
    <div class="container">
      <MainContentCard />
    </div>
  </section>
</template>

<script>
import MainContentCard from "./MainContentCard.vue";
export default {
  name: "HomeMain",
  components: {
    MainContentCard,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/partials/_variables.scss";
.main-content {
  padding: 1rem;
  background-color: black;
}
</style>
