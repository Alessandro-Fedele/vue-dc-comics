<template>
  <div class="container">
    <div class="foot">
      <button>SIGN-UP NOW!</button>
      <div class="social">
        <span>FOLLOW US</span>
        <img src="../assets/footer-facebook.png" alt="Facebook" />
        <img src="../assets/footer-twitter.png" alt="Twitter" />
        <img src="../assets/footer-youtube.png" alt="Youtube" />
        <img src="../assets/footer-pinterest.png" alt="Pinterest" />
        <img src="../assets/footer-periscope.png" alt="Periscope" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterSocial",
};
</script>

<style scoped lang="scss">
.container {
  background-color: #303030;
  padding: 35px 0;
  .foot {
    width: 80%;
    margin: auto;
    display: flex;
    justify-content: space-between;
    .social {
      color: #0282f9;
      font-weight: bolder;
      display: flex;
      align-items: center;
      span {
        padding-right: 10px;
      }
      img {
        padding: 5px;
      }
    }
  }
  button {
    color: white;
    background-color: transparent;
    border: 2px solid #0282f9;
    font-weight: bolder;
    padding: 10px;
    &:hover {
      background-color: #0282f9;
    }
  }
}
</style>