<template>
  <div class="wrapper">
    <div class="jumbo">
      <img
        class="jumbo-img img-fluid w-100"
        src="../assets/img/hero-office.webp"
        alt="office nss presentation"
      />
      <div class="jumbo-text text-center px-3 m-auto">
        <p class="text-uppercase bold upper-text">london collection season</p>
        <h1 class="mt-4 mb-3 display">New Selection Of Henry London</h1>
        <p class="mb-5">
          An estimable experience in the modern collection house
        </p>
        <button type="button" class="btn nss-btn">Discover</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumbotronComponent",
  data() {
    return {};
  },
  methods: {},
  mounted() {},
};
</script>

<style lang='scss' scoped>
.jumbo {
  position: relative;
  .jumbo-img {
    filter: brightness(70%);
    min-height: 600px;
  }
  .jumbo-text {
    width: 100%;
    font-size: 0.7rem;
    .upper-text {
      letter-spacing: 3px;
    }
    color: $nss-bg-lighter;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);

    .display {
      margin: auto;
      width: 500px;
      max-width: 100%;
      font-size: 3.5rem;
    }
    .nss-btn {
      color: $nss-bg-light;
      border: 1px solid $nss-bg-lighter;
      border-radius: 0;
      padding: 0.7rem 6rem;
      outline-color: $nss-bg-lighter;

      &:hover {
        color: black;
        background-color: $nss-bg-lighter;
      }
    }
  }
}
@media screen {
    
}
@media screen and (min-width: 992px) {
 .jumbo-text {
    width: 50%;
 }
}
</style>