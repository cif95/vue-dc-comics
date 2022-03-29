<template>
  <section id="main-jumbo">
    <button class="my-btn-primary">Current Series</button>
  </section>
</template>

<script>
export default {
  name: "MainJumbo",
};
</script>

<style scoped lang="scss">
@import "../../assets/scss/partials/_variables.scss";
section#main-jumbo {
  height: 30vh;
  padding: 5rem;
  position: relative;
  background-image: url("../../assets/img/jumbotron.jpg");
  button {
    top: 95%;
    left: 15%;
    position: absolute;
    font-size: 1.7rem;
  }
}
</style>
