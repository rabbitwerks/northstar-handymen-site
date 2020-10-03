<template>
  <div class="main-sevices--outer">
    <Indoor-Services />
    <Outdoor-Services />
  </div>
</template>

<script>
import indoorServices from '../components/main-services/Indoor_Services.vue';
import outdoorServices from '../components/main-services/Outdoor_Services.vue';
import panelItem from '../components/reusable/Panel_Item.vue';

export default {
  components: {

    'Indoor-Services': indoorServices,
    'Outdoor-Services': outdoorServices,
  },
};
</script>

<style scoped>
.section--banner {
  background-color: #000;
  height: 8rem;
  background-image: url('../assets/img/services/banner-images/indoors_banner_200pxH.jpg');
}
</style>
