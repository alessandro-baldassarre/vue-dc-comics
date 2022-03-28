<template>
  <div>
    <div class="products">
      <div class="container">
        <h3>Content</h3>
      </div>
    </div>
    <div class="menu-buy">
      <div class="container"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndexProducts",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container {
  width: 67%;
  height: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.products {
  height: 100px;
  background-color: rgb(26, 26, 26);
  h3 {
    color: white;
  }
}

.menu-buy {
  height: 110px;
  background-color: rgb(0, 116, 245);
}
</style>
