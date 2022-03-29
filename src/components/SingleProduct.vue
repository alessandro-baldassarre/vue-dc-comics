<template>
  <div class="product-card">
    <div class="img-card">
      <img :src="product.thumb" alt="" />
    </div>
    <h4>{{ product.series }}</h4>
  </div>
</template>

<script>
export default {
  name: "SingleProduct",
  props: {
    product: Object,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/partials/_variables.scss";

.product-card {
  width: calc((100% - 6rem) / 6);
  height: 180px;
  margin: 0.5rem;
  text-align: left;
  .img-card {
    height: 140px;
    overflow: hidden;
    margin-bottom: .8rem;
    img {
      width: 100%;
      object-fit: cover;
    }
    }
    h4 {
      color: white;
      text-transform: uppercase;
      font-size: 0.7rem;
      font-weight: 400;
    }
  
}
</style>
