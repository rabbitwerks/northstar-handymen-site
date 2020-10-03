<template>
  <div
    class="row-item fxbx">
    <div
      class="row-item--image f1">
      <img
        :src="require(`@/assets/img/` + rowData.imgFileName)"
        :alt="rowData.imgAltText"
      >
    </div>
    <div class="row-item--content f4 fxbx fd-c flexgap-3">
      <h1 class="ri-content--header">{{ rowData.headerText }}</h1>
      <div class="ri-content--description j-fe">{{ rowData.panelText }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    rowData: {
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
margin: 0 2rem;
}

.ri-content--header {
  font-size: 2.5rem;
  font-family: 'Archivo Black', sans-serif;
  margin-bottom: .75rem;
  margin-right: 0;
}

.ri-content--description {
  margin-left: 0;
  padding: .6rem 1rem;
  border-radius: .4rem;
  font-size: 1.1rem;
  background-color: rgba(240, 187, 14, 0.45);
}
</style>
