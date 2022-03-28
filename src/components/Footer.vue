<template>
  <div class="home-footer">
    <div class="footer-nav">
      <div class="container"></div>
    </div>
    <div class="footer-social">
      <div class="container"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomeFooter",
};
</script>

<style scoped lang="scss">
div.container {
  width: 70%;
  margin: 0 auto;
  align-items: center;
  justify-content: space-between;
}
div.home-footer {
  div.footer-nav {
    padding: 5rem;
    background-image: url(../assets/img/footer-bg.jpg);
  }
  div.footer-social {
    padding: 2rem;
    background-color: #232323;
  }
}
</style>
