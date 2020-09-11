<template>
  <div class="row-item fxbx">
    <div class="row-item--image f1">
      <img
        :src="require(`@/assets/img/` + panel.imgFileName)"
        :alt="panel.imgAltText"
      >
    </div>
    <div class="row-item--content f4 fxbx fd-c flexgap-3">
      <h1 class="ri-content--header">{{ panel.headerText }}</h1>
      <div class="ri-content--description">{{ panel.panelText }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    panel: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
.row-item--image {
  width: 20%;
}
.row-item--image img {
  width: 100%;
  border: 3px solid var(--grey);
  border-radius: .4rem;
}

.row-item--content {
  margin-left: 2rem;
}

.ri-content--description {
  margin-left: 0;
}
</style>
