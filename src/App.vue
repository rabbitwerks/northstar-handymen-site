<template>
  <div id="app">
    <Nav-Bar />
    <div class="header-banner--container">
      <img src="./assets\img\Linkdin cover.jpg" alt="" class="header-banner--img">
    </div>
    <router-view/>
    <Footer />
  </div>
</template>

<script>
import navBar from './components/nav/Nav_Bar.vue';
import footer from './components/footer/Footer.vue';

export default {
  components: {
    'Nav-Bar': navBar,
    Footer: footer,
  },
};
</script>

<style>
@import url('./assets/css/main.css');
@import url('./assets/css/flexbox-util.css');
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.header-banner--img {
  width: 100%;
}

</style>
