<template>
  <div class="main-sevices--outer">
    <Indoor-Services />

    <!-- <section class="main-services--section" id="serv_outdoors">
      <div class="section--banner">
        <div class="section--header fxbx sp-ctr">
          <h1>Outdoors</h1>
        </div>
      </div>
      <div class="section--main panel--container fxbx sp-ctr flexgap-7">
        <Panel-Item :panelData="panelData.panel_1" />
        <Panel-Item :panelData="panelData.panel_1" />
        <Panel-Item :panelData="panelData.panel_1" />
      </div>
    </section> -->
  </div>
</template>

<script>
import indoorServices from '../components/main-services/Indoor_Services.vue';
import panelItem from '../components/reusable/Panel_Item.vue';

export default {
  // data() {
  //   return {
  //     panelData: {
  //       panel_1: {
  //         navigateRoute: '',
  //         imgFileName: 'services/indoors/carpentry_panel.jpg',
  //         imgAltText: 'Carpentry Stock Photo',
  //         headerText: 'Carpentry and Woodworking',
  //         panelText: `
  //           With over 5 years of carpentry services under our belt,
  //           we can accomplish almost anything you need done, that doesn't require
  //           a full construction crew!
  //         `,
  //       },
  //       panel_2: {
  //         target: '',
  //         imgFileName: 'services/indoors/heat_air_panel.jpg',
  //         imgAltText: 'Heating and Cooling Stock Photo',
  //         headerText: 'Heating and Cooling',
  //         panelText: `
  //           We will strive to make sure your house or business is in perfect climate conditioning.
  //           Whether you need your air cooled or heated, Northstar Handymen will achieve your desired air temp!
  //         `,
  //       },
  //       panel_3: {
  //         target: '',
  //         imgFileName: 'services/indoors/plumbing_panel.jpg',
  //         imgAltText: 'Plumbing Stock Photo',
  //         headerText: 'Plumbing',
  //         panelText: `
  //           Leaky faucets, bad toilets, bath and shower remodels. Kitchen and washroom waterworks.
  //           If water runs through it's pipes then Northstar Handymen can handle it!
  //         `,
  //       },
  //     },
  //   };
  // },
  components: {
    // 'Panel-Item': panelItem,
    'Indoor-Services': indoorServices,
  },
};
</script>

<style scoped>
.main-services--section {
  height: 100vh;
  position: relative;
}

</style>
