<template>
  <div class="home">
    <Hero-Section />
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
        <div class="panel--item f1">
          <a href="" class="panel--img-link">
            <img
              src="../assets/img/panel img/dccdad0439.0.jpeg"
              alt=""
              class="panel--img"
            />
          </a>
          <a href="" class="panel--header-link">
            <h3 class="panel--header">Indoors</h3>
          </a>
            <p>
              We specialize in carpentery, plumbing and drywall.
              We also provide indoor demolition and remodeling services.
              Commercial site work available upon request.
            </p>
        </div>
        <div class="panel--item f1">
          <img
            src="../assets/img/panel img/backyard-landscaping-design.jpg"
            alt=""
            class="panel--img"
          />
          <h3 class="panel--header">Outdoors</h3>
          <p>
            We specialize in carpentery, plumbing and drywall.
            We also provide indoor demolition and remodeling services.
            Commercial site work available upon request.
          </p>
        </div>
        <div class="panel--item f1">
          <img
            src="../assets/img/panel img/Small-Engine-Service-Center-Blog-1.jpg"
            alt=""
            class="panel--img"
          />
          <h3 class="panel--header">Odd Jobs</h3>
          <p>
            We specialize in carpentery, plumbing and drywall.
            We also provide indoor demolition and remodeling services.
            Commercial site work available upon request.
          </p>
        </div>
      </div>
      <h3 class="mission-statement">
        Our mission is to provide top quality workmanship,
        excellent customer service and lasting connections.
      </h3>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import heroSection from '../components/hero-section/Hero_Section.vue';

export default {
  name: 'Home',
  components: {
    'Hero-Section': heroSection,
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
  padding-top: 3rem;
}

</style>
