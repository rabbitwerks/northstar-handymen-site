<template>
  <section class="hero--section">
    <div class="hero--image--container">
      <img
        src="../../assets/img/handyman.jpg"
        alt="Background image of handyman toolbelt"
        class="hero--image"
      />
    </div>
    <div class="hero--inner fxbx">
      <Promo-Heading />
      <Short-Contact-Form />
    </div>
  </section>
</template>

<script>
import promoHeading from './Promo_Heading.vue';
import shortContactForm from './Short_Contact_Form.vue';

export default {
  components: {
    'Promo-Heading': promoHeading,
    'Short-Contact-Form': shortContactForm,
  },
};
</script>

<style scoped>
.hero--section {
  height: 100vh;
  background-color: rgba(0, 0, 0, 1);
}

.hero--image {
  width: 100%;
  max-height: 100vh;
  position: absolute;
  opacity: .5;
}

.hero--inner {
  position: relative;
  z-index: 10;
  width: 70%;
  margin: 0 15%;
  padding: 11rem 0;
}

.short-contact-form {
  background-color: var(--off-white);
  padding: 1rem;
  border: 5px solid var(--grey);
  border-radius: .5rem;
}
</style>
