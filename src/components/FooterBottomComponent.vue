<template>
  <div class="footer-bottom">
    <div class="container">
      <button>SIGN-UP NOW!</button>

      <div class="socials">
        <span>FOLLOW US</span>
        <img src="../assets/img/footer-facebook.png" />
        <img src="../assets/img/footer-twitter.png" />
        <img src="../assets/img/footer-youtube.png" />
        <img src="../assets/img/footer-pinterest.png" />
        <img src="../assets/img/footer-periscope.png" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterBottomComponent",
};
</script>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins" as *;
@use "../assets/styles/partials/variables" as *;

.footer-bottom {
  background-color: $footergrey;
  height: 110px;
  color: $white;
  margin-bottom: 15px;
}

.container {
  height: 110px;
  @include dflex();
}
.socials {
  display: flex;
  align-items: center;
}

img {
  padding-left: 1.2rem;
  cursor: pointer;
}

span {
  color: $skyblue;
  font-weight: bold;
  font-size: 1.3rem;
}

button {
  border: 2px solid $skyblue;
  background-color: transparent;
  color: white;
  padding: 14px 16px;
  font-size: 1.1rem;
  cursor: pointer;
}
</style>
