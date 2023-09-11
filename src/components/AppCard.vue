<script>
export default {
  props: {
    thumb: String,
    series: String,
    price: String,
  },
};
</script>

<template>
  <div class="card">
    <div class="card__img">
      <img :src="thumb" alt="" />
    </div>
    <h4>{{ series }}</h4>
    <p>{{ price }}</p>
  </div>
</template>

<style lang="scss" scoped>

.card {
  width: calc((100% / 6) - .5rem);
  color: white;
}
.card__img > img{
    width: 200px;
    aspect-ratio: 1;
}
</style>
