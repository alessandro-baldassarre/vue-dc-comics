<template>
  <div>
    
    <Jumbotron />

    <Products />

    <Buy />
    
  </div>
</template>

<script>
import Jumbotron from "./Jumbotron.vue";
import Products from "./Products.vue";
import Buy from "./Buy.vue";

export default {
  name: "IndexMain",
  components: {
    Jumbotron,
    Products,
    Buy,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/partials/_variables.scss";

.products {
  height: 100px;
  background-color: $darkGreyBgColor;
  h3 {
    color: white;
  }
}

.menu-buy {
  height: 110px;
  background-color: $primaryColor;
}
</style>
