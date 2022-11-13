<template>
  <div class="col">
    <div class="img-box">
      <img :src="card.thumb" :alt="card.series" />
    </div>
    <div class="caption">
      {{ card.series }}
    </div>
  </div>
</template>

<script>
export default {
  name: "CardComponent",
  props: ["card"],
};
</script>

<style lang="scss" scoped>
.img-box {
  height: 190px;
  margin-top: 60px;
  overflow: hidden;
}

image {
  object-fit: cover;
}
.caption {
  text-transform: uppercase;
  max-width: 190px;
  font-size: 0.9rem;
  margin-top: 15px;
}
</style>
