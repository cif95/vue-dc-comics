<template>
  <div class="card">
    <img :src="cardObject.thumb" :alt="cardObject.series" />
    <h4 class="text-uppercase">{{ cardObject.series }}</h4>
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
  height: 210px;
  margin-bottom: 3rem;
  width: calc(100% / 6 - 2rem);
  img {
    height: 90%;
    width: 100%;
    object-fit: cover;
    object-position: 0% 0%;
  }
  h4 {
    margin: 0.85rem 0;
    font-weight: 400;
  }
}
</style>
