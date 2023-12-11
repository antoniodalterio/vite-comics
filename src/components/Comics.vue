<script>
export default {
  props: {
    img: String,
    title: String,
    priceText: String,
    type: String,
  },
};
</script>
<template>
  <div class="comic">
    <div class="img-container">
      <img :src="img" alt="" />
    </div>
    <h4>{{ title }}</h4>
  </div>
</template>
<style lang="scss" scoped>
.comic {
  width: calc(100% / 6 - 40px);

  .img-container {
    width: 100%;

    img {
      width: 100%;
      display: block;
      height: 200px;
    }
  }

  h4 {
    text-transform: uppercase;
    padding: 10px 0;
    color: white;
  }
}
</style>
