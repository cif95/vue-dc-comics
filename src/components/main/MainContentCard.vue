<template>
  <div class="card">
    <img :src="cardObject.thumb" :alt="cardObject.series" />
    <h6>{{ cardObject.series }}</h6>
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
  height: 200px;
  margin-bottom: 3rem;
  width: calc(100% / 6 - 2rem);
  img {
    height: 90%;
    width: 100%;
    object-fit: cover;
    object-position: 20% 10%;
  }
  h6 {
    margin: 0.85rem 0;
    font-weight: 400;
    text-transform: uppercase;
  }
}
</style>
