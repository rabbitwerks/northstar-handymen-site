<template>
  <div class="nav-item">
    <router-link :to="target">{{ text }}</router-link>
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: true,
    },
    target: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>

.nav-item {
  width: 8rem;
  text-align: center;
  font-family: 'Archivo Black', sans-serif;
}

.nav-item a {
  color: var(--yellow);
  text-decoration: none;
}

.nav-item a:visited {
  color: var(--yellow);
}

.nav-item a:hover {
  color: var(--red);
  border-bottom: 3px solid var(--red);
  transition: color, border 150ms;
}

.nav-item a.router-link-exact-active {
  color: var(--off-white);
}

</style>
