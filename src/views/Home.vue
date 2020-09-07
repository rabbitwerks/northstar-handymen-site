<template>
  <div class="home">
    <Hero-Section />
    <Main-Services-Section />
    <Customer-Testimonies-Section />
  </div>
</template>

<script>
// @ is an alias to /src
import heroSection from '../components/home/hero-section/Hero_Section.vue';
import mainServicesSection from '../components/home/main_services-section/Main_Services_Section.vue';
import customerTestimoniesSection from '../components/home/customer-testimonies-section/Customer_Testimonies_Section.vue';

export default {
  name: 'Home',
  components: {
    'Hero-Section': heroSection,
    'Main-Services-Section': mainServicesSection,
    'Customer-Testimonies-Section': customerTestimoniesSection,
  },
};
</script>

<style scoped>

</style>
