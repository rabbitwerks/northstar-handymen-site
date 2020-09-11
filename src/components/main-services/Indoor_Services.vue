<template>
  <section class="main-services--section" id="serv_indoors">
    <div class="section--banner">
      <div class="section--header fxbx sp-ctr">
        <h1>Indoors</h1>
      </div>
    </div>
    <div class="section--main row-item-container fxbx fd-c sp-ctr fxg-4">
      <div class="row-item fxbx">
        <div class="row-item--image f1">
          <img
            :src="require(`@/assets/img/` + panelData.panel_1.imgFileName)"
            :alt="panelData.panel_1.imgAltText"
          >
        </div>
        <div class="row-item--content f4 fxbx fd-c flexgap-3">
          <h1 class="ri-content--header">{{ panelData.panel_1.headerText }}</h1>
          <div class="ri-content--description">{{ panelData.panel_1.panelText }}</div>
        </div>
      </div>
      <div class="row-item fxbx">
        <div class="row-item--image f1">
          <img
            :src="require(`@/assets/img/` + panelData.panel_2.imgFileName)"
            :alt="panelData.panel_2.imgAltText"
          >
        </div>
        <div class="row-item--content f4 fxbx fd-c flexgap-3">
          <h1 class="ri-content--header">{{ panelData.panel_2.headerText }}</h1>
          <div class="ri-content--description">{{ panelData.panel_2.panelText }}</div>
        </div>
      </div>
      <div class="row-item fxbx">
        <div class="row-item--image f1">
          <img
            :src="require(`@/assets/img/` + panelData.panel_3.imgFileName)"
            :alt="panelData.panel_3.imgAltText"
          >
        </div>
        <div class="row-item--content f4 fxbx fd-c flexgap-3">
          <h1 class="ri-content--header">{{ panelData.panel_3.headerText }}</h1>
          <div class="ri-content--description">{{ panelData.panel_3.panelText }}</div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import panelItem from '../reusable/Panel_Item.vue';

export default {
  //  props: {
  //    panelData: {
  //      type: Object,
  //      required: true,
  //    },
  //  },
  // components: {
  //   'Panel-Item': panelItem,
  // },
  data() {
    return {
      panelData: {
        panel_1: {
          navigateRoute: '',
          imgFileName: 'services/indoors/carpentry_panel.jpg',
          imgAltText: 'Carpentry Stock Photo',
          headerText: 'Carpentry and Woodworking',
          panelText: `
            With over 5 years of carpentry services under our belt,
            we can accomplish almost anything you need done, that doesn't require
            a full construction crew!
          `,
        },
        panel_2: {
          target: '',
          imgFileName: 'services/indoors/heat_air_panel.jpg',
          imgAltText: 'Heating and Cooling Stock Photo',
          headerText: 'Heating and Cooling',
          panelText: `
            We will strive to make sure your house or business is in perfect climate conditioning.
            Whether you need your air cooled or heated, Northstar Handymen will achieve your desired air temp!
          `,
        },
        panel_3: {
          target: '',
          imgFileName: 'services/indoors/plumbing_panel.jpg',
          imgAltText: 'Plumbing Stock Photo',
          headerText: 'Plumbing',
          panelText: `
            Leaky faucets, bad toilets, bath and shower remodels. Kitchen and washroom waterworks.
            If water runs through it's pipes then Northstar Handymen can handle it!
          `,
        },
      },
    };
  },
};
</script>

<style scoped>
.panel--container {
  width: 80%,
}
.section--banner {
  background-color: #000;
  height: 9rem;
  background-image: url('../../assets/img/services/banner-images/indoors_banner_200pxH.jpg');
}

.section--header {
  position: relative;
  z-index: 10;
  height: 100%;
}
.section--header {
  font-size: 3rem;
  background-color: rgba(0, 0, 0, .7);
}

#serv_indoors .section--header {
  color: var(--yellow);
  border-bottom: 7px solid var(--grey);
}
#serv_indoors {
  border-bottom: 7px solid var(--yellow);
}
.section--main {
  padding: 0 15%;
  height: 80%;
}
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
