<template>
  <div class="nav-bar fxbx">
    <Nav-Item target="/" text="HOME" />
    <Nav-Item target="/services" text="SERVICES" />
    <Nav-Item target="/about" text="ABOUT" />
    <Nav-Item target="/gallery" text="GALLERY" />
    <Nav-Item target="/contact" text="CONTACT" />
    <div class="spacer f4"></div>
    <div class="socials f2 fxbx flex-justify-end">
      <div class="phone-number f1">
        651-472-2099
      </div>
    </div>
  </div>
</template>

<script>
import navItem from './Nav_Item.vue';

export default {
  components: {
    'Nav-Item': navItem,
  },
};
</script>

<style scoped>
.nav-bar {
  position: absolute;
  width: 100%;
  padding: 30px;
  font-family: 'Archivo Black', sans-serif;
}

.phone-number {
  font-weight: bold;
  color: var(--yellow);
}

</style>
