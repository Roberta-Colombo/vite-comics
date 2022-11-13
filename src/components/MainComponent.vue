<template>
  <main>
    <div class="container">
      <div class="title">Current Series</div>
      <div class="row">
        <CardComponent
          v-for="(item, index) in cards"
          :key="index"
          :card="item"
        ></CardComponent>
      </div>

      <div class="btn">
        <button>Load More</button>
      </div>
    </div>
  </main>
</template>

<script>
import CardComponent from "./CardComponent.vue";
import { cards } from "../data/all-data.js";

export default {
  name: "MainComponent",
  components: {
    CardComponent,
  },
  data() {
    return {
      cards,
    };
  },
};
</script>

<style lang="scss" scoped>
@use "../assets/styles/partials/mixins" as *;
@use "../assets/styles/partials/variables" as *;

main {
  background-color: $greyblack;
  color: white;
  position: relative;
}

.row {
  display: flex;
  flex-flow: row wrap;
  padding-bottom: 50px;
}

.col {
  flex-basis: calc(100% / 6);
}

button {
  background-color: $skyblue;
  color: white;
  text-transform: uppercase;
  font-weight: bold;
  padding: 10px 40px;
  cursor: pointer;
  border-style: none;
}
.btn {
  text-align: center;
  padding-bottom: 30px;
}

.title {
  background-color: $skyblue;
  height: 60px;
  width: 260px;
  text-transform: uppercase;
  text-align: center;
  line-height: 60px;
  font-size: 1.8rem;
  font-weight: bold;
  position: absolute;
  top: -30px;
}
</style>
