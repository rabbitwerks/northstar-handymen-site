<template>
  <div class="home">
    <Hero-Section />
    <Main-Services-Section />
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

/* main services */
.main-services--section {
  height: 100vh;
  padding: 0 15%;
  text-align: center;
  border-top: 7px solid var(--yellow);
}

.ms--header {
  font-size: 4rem;
  padding: 1.5rem 0 .5rem 0;
}

.ms--subtext {
  font-size: 1.15rem;
  margin: 0 15% 5% 15%;
}

.panel--container {
  width: 100%;
}

.panel--item {
  height: 25rem;
  border: 5px solid var(--grey);
  border-radius: .5rem;
  transition: border 150ms;
  overflow: hidden;
  filter: drop-shadow(0 -.5rem 1rem var(--grey));
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
  border-bottom: 3px solid var(--grey);
}

.panel--img:hover {
  transform: scale(1.1) translateY(-5%);
  border-bottom: 3px solid var(--red);
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

.mission-statement {
  padding-top: 4rem;
}

</style>
