<template>
  <header>
    <HeaderComponent/>
  </header>

  <main>
    <MainComponent/>
  </main>

  <section>
    <BlueBarComponent/>
  </section>

  <footer>
    <FooterTopComponent/>

    <FooterBottomComponent/>
  </footer>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import BlueBarComponent from './components/BlueBarComponent.vue';
import FooterTopComponent from './components/FooterTopComponent.vue';
import FooterBottomComponent from './components/FooterBottomComponent.vue';

  export default {
    components: { 
    HeaderComponent,
    MainComponent,
    BlueBarComponent,
    FooterTopComponent,
    FooterBottomComponent
    }
  }
</script>

<style lang="scss" scoped>

</style>