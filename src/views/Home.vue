<template>
  <div class="home">
    <section class="hero--section">
      <div class="hero--image--container">
        <img src="../assets/img/handyman.jpg" alt="" class="hero--image">
      </div>
      <div class="hero--inner fxbx">
        <div class="promo-heading f2">
          <h1>
            <span class="highlight--yellow">Summer Savings!</span>
            <br>
            <span class="highlight--red">20%</span>
             Off All <span class="highlight--yellow">Landscape</span> and
             <span class="highlight--red">Outdoor Concrete</span> Jobs!</h1>
        </div>
        <div class="short-contact-form f1">
          This is where the contact form will go
        </div>
      </div>
    </section>
    <section class="main-services--section">

    </section>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
};
</script>

<style scoped>

.home {
  border-top: 7px solid #000;
}

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

.promo-heading {
  color: var(--off-white);
  font-size: 3rem;
}

.short-contact-form {
  background-color: var(--off-white);
  padding: 1rem;
  border: 5px solid var(--grey);
  border-radius: 1rem;
}

/* main services */
.main-services--section {
  height: 100vh;
}
</style>
