<template>
  <div class="panel--item f1">
    <a href="" class="panel--img-link">
      <img
        :src="require(`@/assets/img/panel img/` + panelData.imgFileName)"
        :alt="panelData.imgAlt"
        class="panel--img"
      />
    </a>
    <a href="" class="panel--header-link">
      <h3 class="panel--header">{{ panelData.headerText }}</h3>
    </a>
      <p class="panel-text">
        {{ panelData.panelText }}
      </p>
  </div>
</template>

<script>
export default {
  props: {
    panelData: {
      type: Object,
      required: true,
    },
  },

};
</script>

<style scoped>
.panel--item {
  height: 25rem;
  border: 5px solid var(--grey);
  border-radius: .5rem;
  transition: border 150ms;
  overflow: hidden;
  filter: drop-shadow(0 -.5rem 1rem var(--grey));
}

.panel--item:hover {
  border: 5px solid var(--yellow);
}

.panel--item p {
  font-size: 1.1rem;
}

.panel--img {
  width: 100%;
  transition: transform .2s;
  border-bottom: 3px solid var(--grey);
}

.panel--img:hover {
  transform: scale(1.1) translateY(-5%);
  border-bottom: 3px solid var(--red);
}

.panel--header {
  padding: .5rem 0;
  font-size: 1.3rem;
}

.panel--header-link {
  text-decoration: none;
}

.panel--header-link:visited {
  color: var(--black);
}
</style>
