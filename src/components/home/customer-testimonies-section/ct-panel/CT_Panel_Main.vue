<template>
  <div class="ct--panel f1 fxbx flexdir-col ct-1">
    <div class="panel--inner--header fxbx">
      <div class="circle-avatar">
        <img class="avatar-img"
          :src="require('@/assets/img/customer avatars/' + custData.imgName)"
          alt="customer testimony avatar"
        >
      </div>
      <span class="cust--name fxbx sp-ctr">
        {{ custData.name }}
      </span>
    </div>
    <div class="panel--inner--body">
      {{ custData.body }}
    </div>
  </div>
</template>

<script>
export default {
  props: {
    custData: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>

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
