<template>
  <section class="main-services--section">
    <h1 class="ms--header">What We Do</h1>
    <p class="ms--subtext">
      {{ subText }}
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
      {{ missionStatement }}
    </h3>
  </section>
</template>

<script>
import panelItem from './Panel_Item.vue';

export default {
  data() {
    return {
      subText: `Our number one priority is to deliver the finest quality jobs
      in carpentery, landscape, remodeling and demolition.
      Tackling both interior and exterior jobs makes us an extremely versitile crew.
      We also specialize in one-off odd jobs such as small engine repair, lawn care, etc.`,
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
      missionStatement: `Our mission is to provide top quality workmanship,
      excellent customer service and lasting connections.`,
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
  font-family: 'Archivo Black', sans-serif;
}

.ms--subtext {
  font-size: 1.15rem;
  margin: 0 15% 5% 15%;
}

.panel--container {
  width: 100%;
}

.mission-statement {
  padding-top: 4rem;
}
</style>
