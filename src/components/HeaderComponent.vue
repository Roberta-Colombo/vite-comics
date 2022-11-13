<template>
  <header>
    <div class="container">
      <div>
        <img src="../assets/img/dc-logo.png" alt="Logo DC" />
      </div>

      <nav>
        <ul>
          <li v-for="(link, index) in navLinks" :key="index">
            <a href="link.url" :class="{ active: link.active }">{{
              link.text
            }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      navLinks: [
        {
          text: "Characters",
          url: "#",
          active: false,
        },
        {
          text: "Comics",
          url: "#",
          active: false,
        },
        {
          text: "Movies",
          url: "#",
          active: false,
        },
        {
          text: "TV",
          url: "#",
          active: false,
        },
        {
          text: "Games",
          url: "#",
          active: false,
        },
        {
          text: "Collectibles",
          url: "#",
          active: false,
        },
        {
          text: "Videos",
          url: "#",
          active: false,
        },
        {
          text: "Fans",
          url: "#",
          active: false,
        },
        {
          text: "News",
          url: "#",
          active: false,
        },
        {
          text: "Shop",
          url: "#",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins" as *;
@use "../assets/styles/partials/variables" as *;

header {
  background-color: white;
  height: 120px;
  margin-top: 20px;
}

img {
  width: 80%;
}

.container {
  height: 120px;
  @include dflex("between-center");
}

ul {
  li a {
    line-height: 120px;
    text-transform: uppercase;
    display: inline-block;
    padding-right: 1rem;
    padding-left: 1rem;
    color: $darkgrey;
    font-weight: bold;
    font-size: 0.8rem;
    height: 120px;

    &.active,
    &:hover {
      color: $skyblue;
      border-bottom: 5px solid $skyblue;
      width: 100%;
    }
  }
}
</style>
