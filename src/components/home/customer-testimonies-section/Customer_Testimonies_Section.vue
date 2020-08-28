<template>
  <section class="customer-testimonies--section">
    <div class="ct--outer">
      <span class="ct--header">Don't Take Our Word For It...</span>
      <div class="ct--inner fxbx flexgap-7">
        <div class="ct--panel f1 fxbx flexdir-col ct-1">
          <div class="panel--inner--header fxbx">
            <div class="circle-avatar">
              <img class="avatar-img"
                src="@/assets/img/customer avatars/jennifer stock photo.jpg" alt="">
            </div>
            <span class="cust--name fxbx sp-ctr">
              Jennifer M.
            </span>
          </div>
          <div class="panel--inner--body">
            Choosing Northstar Handymen was the best desicion I made this year!
            Not only were my deck stairs repaired but the job was done fast and very affordably.
            Definitely recommending these guys!
          </div>
        </div>
        <div class="ct--panel f1 fxbx flexdir-col ct-1">
          <div class="panel--inner--header fxbx">
            <div class="circle-avatar">
              <img class="avatar-img"
                src="@/assets/img/customer avatars/eddie stock photo.jpg" alt="">
            </div>
            <span class="cust--name fxbx sp-ctr">
              Eddie T.
            </span>
          </div>
          <div class="panel--inner--body">
            Choosing Northstar Handymen was the best desicion I made this year!
            Not only were my deck stairs repaired but the job was done fast and very affordably.
            Definitely recommending these guys!
          </div>
        </div>
        <div class="ct--panel f1 fxbx flexdir-col ct-1">
          <div class="panel--inner--header fxbx">
            <div class="circle-avatar">
              <img class="avatar-img"
                src="../../../assets/img/customer avatars/oldies stock photo.jpg" alt="">
            </div>
            <span class="cust--name fxbx sp-ctr">
              Jan & Jerry
            </span>
          </div>
          <div class="panel--inner--body">
            Choosing Northstar Handymen was the best desicion I made this year!
            Not only were my deck stairs repaired but the job was done fast and very affordably.
            Definitely recommending these guys!
          </div>
        </div>

      </div>
    </div>
  </section>
</template>

<script>
export default {

};
</script>

<style scoped>

.customer-testimonies--section {
  height: 100vh;
  background-color: #ddd;
  border-top: 7px solid var(--red);
}

.ct--outer {
  padding: 2% 15%;
}

.ct--header {
  font-size: 4rem;
  color: var(--black);
  font-family: 'Archivo Black', sans-serif;
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
</style>
