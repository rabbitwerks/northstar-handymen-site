<template>
  <section class="main-services--section">
    <h1 class="ms--header">What We Do</h1>
    <p class="ms--subtext">
      Our number one priority is to deliver the finest quality jobs
      in carpentery, landscape, remodeling and demolition.
      Tackling both interior and exterior jobs makes us an extremely versitile crew.
      We also specialize in one-off odd jobs such as small engine repair, lawn care, etc.
      <br />
      Call now for a free estimate!
    </p>
    <div class="panel--container fxbx flexgap-7">

      <Panel-Item
        :panelData="panelData.panel_1"
      />
      <Panel-Item
        :panelData="panelData.panel_2"
      />
      <Panel-Item
        :panelData="panelData.panel_3"
      />

    </div>
    <h3 class="mission-statement">
      Our mission is to provide top quality workmanship,
      excellent customer service and lasting connections.
    </h3>
  </section>
</template>

<script>
import panelItem from './Panel_Item.vue';

export default {
  data() {
    return {
      panelData: {
        panel_1: {
          target: '',
          imgFileName: 'dccdad0439.0.jpeg',
          imgAlt: 'indoors remodel stock photo',
          headerText: 'Indoors',
          panelText: 'We specialize in carpentery, plumbing and drywall. We also provide indoor demolition and remodeling services. Commercial site work available upon request.',
        },
        panel_2: {
          target: '',
          imgFileName: 'backyard-landscaping-design.jpg',
          imgAlt: 'outdoor patio stock photo',
          headerText: 'Outdoors',
          panelText: 'We specialize in carpentery, plumbing and drywall. We also provide indoor demolition and remodeling services. Commercial site work available upon request.',
        },
        panel_3: {
          target: '',
          imgFileName: 'Small-Engine-Service-Center-Blog-1.jpg',
          imgAlt: 'lawn mower repair stock photo',
          headerText: 'Odd Jobs',
          panelText: 'We specialize in carpentery, plumbing and drywall. We also provide indoor demolition and remodeling services. Commercial site work available upon request.',
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
