<template>
  <div class="container">
    <div class="card-container">
      <div class="card" v-for="(image, i) in cardList" :key="i">
        <img :src="image.imgUrl" :alt="image.text" />
        <span>{{ image.text }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BluBar",
  data() {
    return {
      cardList: [
        {
          text: "Digital Comics",
          imgUrl: require("../assets/buy-comics-digital-comics.png"),
        },
        {
          text: "Dc Merchandise",
          imgUrl: require("../assets/buy-comics-merchandise.png"),
        },
        {
          text: "Subscription",
          imgUrl: require("../assets/buy-comics-subscriptions.png"),
        },
        {
          text: "Comic Shop Locator",
          imgUrl: require("../assets/buy-comics-shop-locator.png"),
        },
        {
          text: "dc Power Visa",
          imgUrl: require("../assets/buy-dc-power-visa.svg"),
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.container {
  background-color: #0282f9;
  .card-container {
    width: 80%;
    margin: auto;
    display: flex;
    padding: 35px 10px;
    .card {
      width: 20%;
      color: white;
      display: flex;
      align-items: center;
      text-transform: uppercase;
      img {
        width: 50px;
        padding-right: 8px;
      }
    }
  }
}
</style>