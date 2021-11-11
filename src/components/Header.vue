<template>
  <header class="container">
    <div class="logo">
      <img src="../assets/dc-logo.png" alt="Dc-logo" />
    </div>
    <nav>
      <ul>
        <li v-for="(item, i) in navLinks" :key="i">
          <a :href="item.href">{{ item.title }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      navLinks: [
        {
          title: "Characters",
          href: "#",
        },
        {
          title: "Comics",
          href: "#",
        },
        {
          title: "Movies",
          href: "#",
        },
        {
          title: "TV",
          href: "#",
        },
        {
          title: "Games",
          href: "#",
        },
        {
          title: "Collectibles",
          href: "#",
        },
        {
          title: "Videos",
          href: "#",
        },
        {
          title: "Fans",
          href: "#",
        },
        {
          title: "News",
          href: "#",
        },
        {
          title: "Shop",
          href: "#",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.container {
  margin: auto;
  width: 80%;
  display: flex;
  justify-content: space-between;
  .logo {
    padding: 20px 0;
  }
  ul {
    display: flex;
    align-items: center;
    height: 100%;
    margin: 0;
    li {
      list-style: none;
      text-transform: uppercase;
      a {
        text-decoration: none;
        padding: 62px 15px;
        color: black;
        font-weight: bold;
        font-size: 15px;
        display: block;
        &:hover {
          color: #0282f9;
          border-bottom: 5px solid #0282f9;
        }
      }
    }
  }
}
</style>