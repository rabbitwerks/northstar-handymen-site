<template>
  <footer class="app-footer">
    <div class="footer--main fxbx flexgap-7">
      <div class="footer--logo f1 fxbx sp-ctr">
        <h1 class="footer--header">
          <span class="highlight--yellow">
            Northstar
          </span>
          <span class="highlight--red">
            Handymen
          </span>
        </h1>
      </div>
      <div class="links--site f2 fxbx fd-c txt-right">
      <a href="./views/Home.vue" class="site-link f1">
          Home
        </a>
        <a href="#" class="site-link f1">
          Services
        </a>
        <a href="./views/About.vue" class="site-link f1">
          About
        </a>
        <a href="#" class="site-link f1">
          Gallery
        </a>
        <a href="#" class="site-link f1">
          Contact
        </a>
      </div>
      <div class="links--social f2 fxbx fd-c">
        <a href="mailto:northstarhandymen@gmail.com" class="resource-link f1">
          Email
        </a>
        <a href="https://www.facebook.com/northstarhandymen" class="resource-link f1">
          Facebook
        </a>
        <a href="#" class="resource-link f1">
          Site Map
        </a>
        <a href="#" class="resource-link f1">
          Privacy Policy
        </a>
        <a href="#" class="resource-link f1">
          Liability Restrictions and Exemptions
        </a>
      </div>
    </div>
    <div class="footer--legal fxbx fd-c sp-ctr">
      <span class="copyright">
        &copy; 2020 Northstar Handymen LLC. All Rights Reserved.
      </span>
      <span class="credit">
        Rabbitwerks Javascript
      </span>
    </div>
  </footer>
</template>

<script>
export default {

};
</script>

<style scoped>
.app-footer {
  height: 20rem;
  padding: 5rem 15%;
  background-color: var(--black);
  color: var(--grey);
  border-top: 7px solid var(--red);
}

.app-footer a {
  text-decoration: none;
  color: var(--grey)
}

.app-footer a:hover {
  color: var(--yellow);
}

.footer--header {
  font-size: 4rem;
}

.txt-right {
  text-align: right;
}

.links--social {
  margin-right: 1rem;
}

.footer--legal {
  height: 50%;
  font-size: .8rem;
  text-align: center;
}
.copyright {
  margin: .5rem 0;
}
</style>
