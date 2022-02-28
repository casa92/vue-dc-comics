<template>
  <div id="app">
    <Header/>
    <Banner/>
    <Main/>
    <Footer/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Banner from "./components/Banner.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Banner,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">

@import './style/general.scss';

// #app {
//   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
//   margin-top: 60px;
// }
</style>
