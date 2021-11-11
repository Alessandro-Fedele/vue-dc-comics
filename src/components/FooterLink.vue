<template>
  <div class="container">
    <div class="bg"><img src="../assets/footer-bg.jpg" alt="background" /></div>
    <div class="list-container">
      <div>
        <div>
          <h2>Dc Comics</h2>
          <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
        </div>
        <div>
          <h2>Shop</h2>
          <ul>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
      </div>
      <div>
        <h2>DC</h2>
        <ul>
          <li><a href="#">Terms Of Use</a></li>
          <li><a href="#">Privacy policy (New)</a></li>
          <li><a href="#">Ad Choise</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </div>
      <div>
        <h2>Sites</h2>
        <ul>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>
    </div>
    <img class="logo" src="../assets/dc-logo-bg.png" alt="Dc-Logo" />
  </div>
</template>

<script>
export default {
  name: "FooterLink",
};
</script>

<style scoped lang="scss">
.container {
  position: relative;
  padding: 50px 0 30px 0;
  .bg {
    img {
      position: absolute;
      top: 0;
      z-index: -1;
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
  .list-container {
    width: 80%;
    margin: auto;
    display: flex;
  }
  h2 {
    text-transform: uppercase;
    color: white;
    padding-bottom: 10px;
  }
  ul {
    padding-bottom: 20px;
  }
  li {
    list-style: none;
    padding: 5px;
    margin-right: 50px;
    padding-left: 0;
    a {
      color: #8a8989;
      text-decoration: none;
      &:hover {
        color: white;
      }
    }
  }
  .logo {
    position: absolute;
    top: 0;
    transform: scale(1.2);
    top: -60px;
    right: 350px;
    z-index: -1;
  }
}
</style>