<template>
  <section class="blue-bar">
    <div class="container">
      <nav>
        <ul>
          <li v-for="(section, index) in sectionMenu" :key="index">
            <img :src="section.src" :alt="section.text" />
            <span>
              <a :href="section.url">{{ section.text }}</a>
            </span>
          </li>
        </ul>
      </nav>
    </div>
  </section>
</template>

<script>
export default {
  name: "BlueBarComponent",
  data() {
    return {
      sectionMenu: [
        {
          text: "DIGITAL COMICS",
          src: "../../img_copy/buy-comics-digital-comics.png",
          url: "#",
        },
        {
          text: "DC MERCHANDISE",
          src: "../../img_copy/buy-comics-merchandise.png",
          url: "#",
        },
        {
          text: "SUBSCRIPTION",
          src: "../../img_copy/buy-comics-subscriptions.png",
          url: "#",
        },
        {
          text: "COMIC SHOP LOCATOR",
          src: "../../img_copy/buy-comics-shop-locator.png",
          url: "#",
        },
        {
          text: "DC POWER VISA",
          src: "../../img_copy/buy-dc-power-visa.svg",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins" as *;
@use "../assets/styles/partials/variables" as *;

.blue-bar {
  background-color: $skyblue;
  height: 160px;
  color: $white;
  @include dflex("center-center");
}

ul {
  justify-content: space-evenly;
}

li {
  @include dflex("center-center");

  a {
    color: $white;
    font-size: 0.9rem;
  }
}

img {
  height: 30%;
  padding-right: 1rem;
}
</style>
