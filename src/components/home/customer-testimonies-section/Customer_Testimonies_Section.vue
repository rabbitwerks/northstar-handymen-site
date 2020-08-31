<template>
  <section class="customer-testimonies--section">
    <div class="ct--outer">
      <h1 class="ct--header">
        Don't
        <span class="highlight--yellow stroke--black">Take Our Word</span>
        For It...
      </h1>
      <h2 class="subtext">
        Check out what
        <span class="highlight--red">our customers</span> have to say!
      </h2>
      <div class="ct--inner fxbx flexgap-7">

        <CT-Panel
          :custData="custTestsData.cust_1"
        />
        <CT-Panel
          :custData="custTestsData.cust_2"
        />
        <CT-Panel
          :custData="custTestsData.cust_3"
        />

      </div>
        <div class="after-text fxbx sp-ctr">
          <h3>
            Rest assured that with Northstar Handymen you be getting the best quality work
            for the best value in town.
          </h3>
        </div>
    </div>
  </section>
</template>

<script>
import ctPanel from './ct-panel/CT_Panel_Main.vue';

export default {
  data() {
    return {
      custTestsData: {
        cust_1: {
          name: 'Jennifer M.',
          body: `Choosing Northstar Handymen was the best desicion I made this year!
            Not only were my deck stairs repaired but the job was done fast and very affordably.
            Definitely recommending these guys!`,
          imgName: 'jennifer stock photo.jpg',
        },
        cust_2: {
          name: 'Eddie T.',
          body: `Fast, efficient, reliable and affordable.
            My 4 favorite things when I look for a handyman to do some projects for me.
            Super friendly and willing to accomodate requests. 10 out of 10.`,
          imgName: 'eddie stock photo.jpg',
        },
        cust_3: {
          name: 'Jan & Jerry',
          body: `Matt and Abe helped us to find the best solution for our
            three-season porch renovation while keeping the costs as budget friendly as possible.
            The results were outstanding and we couldn't be happier. Thank you Northstar Handymen!`,
          imgName: 'oldies stock photo.jpg',
        },
      },
    };
  },
  components: {
    'CT-Panel': ctPanel,
  },
};
</script>

<style scoped>

.customer-testimonies--section {
  height: 100vh;
  background-color: #ddd;
  border-top: 7px solid var(--yellow);
}

.ct--outer {
  padding: 2% 15%;
}

.ct--header {
  font-size: 4rem;
  color: var(--black);
  font-family: 'Archivo Black', sans-serif;
}

.subtext {
  text-align: right;
  -webkit-text-stroke: px #000;
}

.ct--inner {
  width: 100%;
}

.ct--panel {
  margin-top: 5rem;
  height: 20rem;
  border: 5px solid var(--yellow);
  border-radius: 50%;
  background-color: var(--off-white);
  filter: drop-shadow(0 -.5rem 1rem var(--grey));
  position: relative;
}

.circle-avatar {
  height: 6rem;
  width: 6rem;
  border-radius: 50%;
  background-color: #fff;
}

.avatar-img {
  height: 100%;
  border: 3px solid var(--red);
  border-radius: 50%;
}

.cust--name {
  padding: 0 .5rem;
  font-family: 'Archivo Black', sans-serif;
  font-size: 1.5rem;
}

.panel--inner--body {
  padding: 1rem 2rem 0 2rem;
  text-align: center;
}

.after-text {
  padding: 6rem;
  font-size: 1.35rem;
  text-align: center;
}
</style>
