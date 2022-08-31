<template>
  <div id="app">
    <h1 class="bold">Hello</h1>
    <h1 class="regular-2">Hello</h1>
    <h1 class="display">Hello</h1>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
};
</script>

<style lang="scss">
@font-face {
  font-family: "Montserrat-Regular";
  src: local("Montserrat-Regular"),
    url(./fonts/Montserrat-Regular.ttf) format("truetype");
}
@font-face {
  font-family: "Montserrat-Bold";
  src: local("Montserrat-Bold"),
    url(./fonts/Montserrat-Bold.ttf) format("truetype");
}
@font-face {
  font-family: "Miller-Display";
  src: local("Miller-Display_30501"),
    url(./fonts/Miller-Display_30501.ttf) format("truetype");
}
@font-face {
  font-family: "Merriweather-Regular";
  src: local("Merriweather-Regular"),
    url(./fonts/Merriweather-Regular.ttf) format("truetype");
}
#app {
  font-family: "Montserrat-Regular", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.bold {
  font-family: "Montserrat-Bold", Helvetica, Arial, sans-serif;
}
.display {
  font-family: "Miller-Display", Helvetica, Arial, sans-serif;
}
.regular-2 {
  font-family: "Merriweather-Regular", Helvetica, Arial, sans-serif;
}
</style>
