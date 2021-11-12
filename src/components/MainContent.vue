<template>
  <main class="container">
    <img src="../assets/jumbotron.jpg" alt="dc-hero" />
    <div class="current-series">
      <button>Current Series</button>
    </div>
    <ComicCard></ComicCard>
    <div class="btn-container">
      <button>Load More</button>
    </div>
  </main>
</template>

<script>
import ComicCard from "@/components/ComicCard.vue";
export default {
  name: "MainContent",
  components: {
    ComicCard,
  },
};
</script>

<style scoped lang="scss">
.container {
  background-color: #1c1c1c;
  img {
    width: 100%;
    object-fit: cover;
    height: 400px;
    object-position: top;
  }
  .current-series {
    position: relative;
    button {
      position: absolute;
      top: -25px;
      left: 170px;
      color: white;
      font-size: 25px;
      background-color: #0282f9;
      border: 3px solid #0282f9;
      font-weight: bolder;
      padding: 5px 15px;
    }
  }
  .btn-container {
    text-align: center;
    padding-bottom: 30px;
    button {
      color: white;
      font-size: 15px;
      background-color: #0282f9;
      border: 3px solid #0282f9;
      font-weight: bolder;
      padding: 8px 50px;
      margin-top: 60px;
      &:hover {
        border: 3px solid white;
      }
    }
  }
}
</style>