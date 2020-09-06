<template>
  <div class="main-sevices--outer">
    <section class="main-services--indoors">
      <div class="section--banner">
        <div class="section--header fxbx sp-ctr">
          <h1>Indoors</h1>
        </div>
      </div>
      <div class="section--main panel--container fxbx sp-ctr flexgap-7">
        <Panel-Item :panelData="panelData.panel_1" />
        <Panel-Item :panelData="panelData.panel_1" />
        <Panel-Item :panelData="panelData.panel_1" />
      </div>
    </section>
  </div>
</template>

<script>
import panelItem from '../components/reusable/Panel_Item.vue';

export default {
  data() {
    return {
      panelData: {
        panel_1: {
          target: '#',
          imgFileName: 'services/banner-images/indoors_banner_200pxH.jpg',
          imgAltText: 'Carpentry Stock Photo',
          headerText: 'Carpentry',
          panelText: `With over 5 years of carpentry services under our belt,
            we can accomplish almost anything you need done, that doesn't require
            a full construction crew!`,
        },
      },
    };
  },
  components: {
    'Panel-Item': panelItem,
  },
};
</script>

<style scoped>
.main-services--indoors {
  height: 100vh;
  position: relative;
}
.section--banner {
  background-color: #000;
  height: 10rem;
  background-image: url('../assets/img/site images/indoors_banner_200pxH.jpg');
}

.section--header {
  position: relative;
  z-index: 10;
  color: var(--yellow);
  height: 100%;
}
.section--header {
  font-size: 3rem;
  background-color: rgba(0, 0, 0, .7);
}

.section--main {
  padding: 0 15%;
  height: 80%;
}
</style>
