<template>
  <section class="main-services--section" id="serv_indoors">
    <div class="section--banner">
      <div class="section--header fxbx sp-ctr">
        <h1>Indoors</h1>
      </div>
    </div>
    <div
      class="section--main row-item--container fxbx fd-c sp-ctr fxg-4"

      >
      <Row-Item
        :rowData="rowData.panel_1"
      />
      <Row-Item
        :rowData="rowData.panel_2"
      />
      <Row-Item
        :rowData="rowData.panel_3"

      />
    </div>
  </section>
</template>
<script>

import rowItem from '../reusable/Row_Item.vue';

export default {
  components: {
    'Row-Item': rowItem,
  },
  data() {
    return {
      rowData: {
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
        renderDirection: 'right',
      },
    };
  },
};
</script>

<style scoped>
.main-services--section {
  height: 100vh;
  position: relative;
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
  font-size: 3rem;
  background-color: rgba(0, 0, 0, .7);
}

.section--main {
  padding: 0 15%;
  height: 80%;
}

#serv_indoors .section--header {
  color: var(--yellow);
  border-bottom: 7px solid var(--grey);
}
#serv_indoors {
  border-bottom: 7px solid var(--yellow);
}

#serv_outdoors .section--header {
  color: var(--red);
  border-bottom: 7px solid var(--grey);
}

</style>
