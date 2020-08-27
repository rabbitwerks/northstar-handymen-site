<template>
  <div class="home">
    <Hero-Section />
    <Main-Services-Section />
    <section class="customer-testimonies--section">
      <div class="ct--outer">
        <span class="ct--header">Don't Take Our Word For It...</span>
        <div class="ct--inner fxbx flexgap-7">
          <div class="ct--panel f1 ct-1">
            <div class="panel--inner--header fxbx">
              <div class="circle-avatar"></div>
              <div class="cust--name"></div>
              one
            </div>
          </div>
          <div class="ct--panel f1 ct-2">two</div>
          <div class="ct--panel f1 ct-3">three</div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import heroSection from '../components/home/hero-section/Hero_Section.vue';
import mainServicesSection from '../components/home/main_services-section/Main_Services_Section.vue';

export default {
  name: 'Home',
  components: {
    'Hero-Section': heroSection,
    'Main-Services-Section': mainServicesSection,
  },
};
</script>

<style scoped>

.home {
  border-top: 7px solid var(--black);
}

.customer-testimonies--section {
  height: 100vh;
  background-color: var(--grey);
  border-top: 7px solid var(--red);
}

.ct--outer {
  padding: 2% 15%;
}

.ct--header {
  font-size: 4rem;
  color: var(--yellow);
  border-bottom: 7px solid var(--yellow);
  font-family: 'Archivo Black', sans-serif;
}

.ct--inner {
  width: 100%;
}

.ct--panel {
  margin-top: 5rem;
  height: 20rem;
  border: 5px solid var(--black);
  border-radius: .5rem;
  background-color: var(--off-white);
  filter: drop-shadow(0 -1rem 1rem #fff);
  position: relative;
}

.circle-avatar {
  height: 6rem;
  width: 6rem;
  border: 3px solid var(--black);
  border-radius: 50%;
}

</style>
