<template>
  <div class="card">
    <img :src="cardObject.thumb" :alt="cardObject.series" />
    <h5>{{ cardObject.series }}</h5>
  </div>
</template>

<script>
export default {
  name: "MainContentCard",
  props: { cardObject: Object },
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/partials/_variables.scss";
div.card {
  border: 1rem solid $secondaryColor;
  width: calc(100% / 6 - 2rem);
  img {
    height: 200px;
    width: 200px;
    object-fit: cover;
    object-position: 20% 10%;
  }
}
</style>
