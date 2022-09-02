<template>
  <div id="app">
    <div class="container">
      <navbar-component></navbar-component>
      <main>
        <jumbotron-component></jumbotron-component>
      </main>
    </div>
  </div>
</template>

<script>
import JumbotronComponent from './components/Jumbotron.vue';
import NavbarComponent from "./components/Navbar.vue";
export default {
  name: "App",
  components: {
    NavbarComponent,
    JumbotronComponent,
  },
};
</script>

<style lang="scss">
@import "@/assets/scss/variables.scss";
@import "@/assets/scss/style.scss";
</style>
