<template>
  <div id="jumbotron">
  </div>
</template>

<script>
export default {
  name: "MainProducts",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/partials/_variables.scss";

#jumbotron{
  height: 300px;
  background-image: url("../assets/img/jumbotron.jpg");
  background-size: cover;
}
</style>
