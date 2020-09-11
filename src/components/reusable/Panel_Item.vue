<template>
  <div class="panel--item f1">
    <router-link
      v-if="panelData.navigateRoute"
      :to="panelData.navigateRoute"
      class="panel--img-link"
    >
      <img
        :src="require(`@/assets/img/` + panelData.imgFileName)"
        :alt="panelData.imgAlt"
        class="panel--img"
      />
    </router-link>
    <img
      v-else
      :src="require(`@/assets/img/` + panelData.imgFileName)"
      :alt="panelData.imgAlt"
      class="panel--img"
    />
    <router-link
      v-if="panelData.navigateRoute"
      :to="panelData.navigateRoute"
      class="panel--header-link"
    >
      <h3
        class="panel--header"
        >{{ panelData.headerText }}
      </h3>
    </router-link>
    <h3
      v-else
      class="panel--header"
      >{{ panelData.headerText }}
    </h3>
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
  transition: all 150ms linear;
  overflow: hidden;
  filter: drop-shadow(0 -.5rem 1rem var(--grey));
  text-align: center;
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
  border-bottom: 4px solid var(--grey);
}

.panel--img:hover {
  transform: scale(1.1) translateY(-5%);
  border-bottom: 4px solid var(--red);
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
