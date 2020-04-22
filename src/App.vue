<template>
  <div id="app">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <router-link class="navbar-item" to="/">
          Armaan Lala
        </router-link>

        <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample" :class="{ 'is-active': showNav }" @click="showNav = !showNav">
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div id="navbarBasicExample" class="navbar-menu" :class="{ 'is-active': showNav }">
        <div class="navbar-start">

        </div>

        <div class="navbar-end">
          <router-link to="/" class="navbar-item">
            Home
          </router-link>
          <router-link to="/about" class="navbar-item">
           About
          </router-link>
          <router-link to="/projects" class="navbar-item">
           Projects
          </router-link>
          <router-link to="/contact" class="navbar-item">
           Contact
          </router-link>
       </div>
     </div>
   </nav>
   <router-view />
   <footer class="footer">
    <div class="content has-text-centered">
      <p>
        Armaan Lala 2020
      </p>
      <p>
        Armaan Lala 2020
      </p>
      <p>
        Armaan Lala 2020
      </p>
    </div>
  </footer>
</div>
</template>

<script>
  export default {
    name: "App",
    data() {
      return{
        showNav: false
      }
    },
  };
</script>

<style type="text/css">
#app {
  /* padding-top: 40px; */
  min-height: 100vh;
  overflow: hidden;
  display: block;
  position: relative;
  padding-bottom: 152px; 
}
footer {
 position: absolute;
 bottom: 0;
 width: 100%;
 min-height: fit-content;
}
.footer {
  padding:1.5rem!important;
}
a {
  font-size: 1.4rem;
}
</style>

<style lang="sass">
@import "~bulma/bulma.sass"
</style>