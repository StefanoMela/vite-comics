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
    <h5>{{ series }}</h5>
    <p>{{ price }}</p>
  </div>
</template>

<style lang="scss" scoped>
.card__img > img{
    width: 300px;
    aspect-ratio: 1;
}
</style>
