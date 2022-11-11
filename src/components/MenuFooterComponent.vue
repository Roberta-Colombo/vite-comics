<template>
  <div class="footer-menus">
    <h4>{{ item.title }}</h4>
    <nav>
      <ul>
        <li v-for="(link, index) in item.links" :key="index">
          <a :href="link.url">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "MenuFooterComponent",
  props: ["item"],
};
</script>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins" as *;
@use "../assets/styles/partials/variables" as *;

ul {
  display: block;

  li a {
    color: grey;
    font-size: 0.8rem;
    line-height: 1.3rem;
  }
}
.footer-menus {
  padding-top: 3rem;
  padding-bottom: 3rem;
  padding-right: 1.5rem;

  h4 {
    text-transform: uppercase;
    padding-bottom: 0.8rem;
    font-size: 1.2rem;
  }
}
</style>
