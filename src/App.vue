<template>
  <div id="app">
    <Header></Header>
    <MainContent></MainContent>
    <BlueBar></BlueBar>
    <FooterLink></FooterLink>
    <FooterSocial></FooterSocial>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import MainContent from "./components/MainContent.vue";
import BlueBar from "./components/BlueBar.vue";
import FooterLink from "./components/FooterLink.vue";
import FooterSocial from "./components/FooterSocial.vue";

export default {
  name: "App",
  components: {
    Header,
    MainContent,
    BlueBar,
    FooterLink,
    FooterSocial,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
