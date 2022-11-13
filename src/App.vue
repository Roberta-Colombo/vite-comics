<template>
  <header>
    <HeaderComponent />
  </header>

  <div>
    <JumbotronComponent />
  </div>

  <main>
    <MainComponent />
  </main>

  <section>
    <BlueBarComponent />
  </section>

  <footer>
    <FooterTopComponent />

    <FooterBottomComponent />
  </footer>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import BlueBarComponent from "./components/BlueBarComponent.vue";
import FooterTopComponent from "./components/FooterTopComponent.vue";
import FooterBottomComponent from "./components/FooterBottomComponent.vue";
import JumbotronComponent from "./components/JumbotronComponent.vue";

export default {
  components: {
    HeaderComponent,
    MainComponent,
    BlueBarComponent,
    FooterTopComponent,
    FooterBottomComponent,
    JumbotronComponent,
  },
};
</script>

<style lang="scss" scoped></style>
