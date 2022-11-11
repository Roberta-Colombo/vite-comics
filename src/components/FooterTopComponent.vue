<template>
  <div class="footer-top">
    <div class="container">
      <div class="left-footer">
        <MenuFooterComponent
          v-for="(menu, index) in menus"
          :key="index"
          :item="menu"
        />
      </div>

      <img src="../assets/img/dc-logo-bg.png" alt="Logo DC" />
    </div>
  </div>
</template>

<script>
import { footerMenu } from "../data/all-data";
import MenuFooterComponent from "./MenuFooterComponent.vue";
export default {
  name: "FooterTopComponent",
  components: {
    MenuFooterComponent,
  },
  data() {
    return {
      menus: footerMenu,
    };
  },
};
</script>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins" as *;
@use "../assets/styles/partials/variables" as *;

.footer-top {
  background-image: url("../assets/img/footer-bg.jpg");
  height: 400px;
  color: $white;
  overflow: hidden;
}

img {
  position: absolute;
  bottom: -30%;
  left: 57%;
}

.container {
  position: relative;
}

.left-footer {
  display: flex;
}
</style>
