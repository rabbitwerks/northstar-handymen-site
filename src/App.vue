<template>
  <div id="app">
    <div id="nav" class="fxbx">
      <div class="nav-item">
        <router-link to="/">Home</router-link>
      </div>
      <router-link to="/about">About</router-link>
      <router-link to="/about">Gallery</router-link>
      <router-link to="/about">Contact</router-link>
    </div>
    <div class="hero--img-container">
      <img src="./assets\img\Linkdin cover.jpg" alt="" class="hero--img">
    </div>
    <router-view/>
  </div>
</template>

<style>
@import url('./assets/css/main.css');
@import url('./assets/css/flexbox-util.css');
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

#nav {
  position: absolute;
  width: 100%;
  padding: 30px;
  background-color: var(--black);
}

.nav-item {
  width: 6rem;
}
#nav a {
  font-weight: bold;
  color: var(--yellow);
}

#nav a:hover {
  color: var(--red);
}

#nav a.router-link-exact-active {
  color: var(--red);
}

.hero--img {
  width: 100%;
}
</style>
