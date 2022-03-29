<template>
  <div>
    <div class="menu-buy">
      <div class="my-container">
        <div v-for="(element, index) in buyElement" :key="index" class="buy-card">
          <img :src="require(`../assets/img/${element.imgUrl}`)" alt="" />
          <h4>{{element.name}}</h4>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainBuy",
  data: function () {
    return {
      buyElement: [
        {
          name: "digital comics",
          imgUrl: "buy-comics-digital-comics.png",
        },
        {
          name: "dc merchandise",
          imgUrl: "buy-comics-merchandise.png",
        },
        {
          name: "subscription",
          imgUrl: "buy-comics-subscriptions.png",
        },
        {
          name: "comic shop locator",
          imgUrl: "buy-comics-shop-locator.png",
        },
        {
          name: "dc power visa",
          imgUrl: "buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/partials/_variables.scss";

.menu-buy {
  height: 110px;
  background-color: $primaryColor;
  .buy-card {
    display: flex;
    align-items: center;
    height: 100%;
    margin-right: 1rem;
    img {
      height: 40%;
      margin-right: 0.5rem;
    }
    h4 {
      color: white;
      text-transform: uppercase;
      font-size: 0.7rem;
      font-weight: 400;
    }
  }
}
</style>
