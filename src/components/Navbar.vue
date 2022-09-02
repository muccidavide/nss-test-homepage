<template>
  <header>
    <nav class="navbar navbar-expand navbar-light p-0">
      <ul class="nav navbar-nav nav-left">
        <li class="nav-item bold nss-bg-primary py-2 px-3">
          <a class="nav-link active text-white fs-3" href="#" aria-current="page"
            >WATCH/LAB<span class="visually-hidden">(current)</span></a
          >
        </li>
      </ul>
      <ul
        class="
          nav
          navbar-nav
          nav-center
          justify-content-between
          flex-nowrap
          bold
        "
      >
        <li class="nav-item" v-for="link in links" :key="link">
          <a class="nav-link text-dark" href="#">{{ link }}</a>
        </li>
      </ul>
      <div class="nav navbar-nav nav-right">
        <div
          class="search-bar d-flex justify-content-center align-items-center py-2 px-3"
        >
          <input class="search-space me-3" /><i class="bi bi-search bi-bold"></i>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  name: "NavbarComponent",
  data() {
    return {
      links: ["About us", "Brand", "Projects", "Magazine", "Press", "Contacts"],
    };
  },
  methods: {},
  mounted() {},
};
</script>

<style lang='scss' scoped>
.navbar {
  .nav-link:hover {
    color: $nss-text-primary;
  }
  .nav-center {
    width: 100%;
    max-width: 900px;
    margin: auto;
    padding: 0 5%;
    a {
      font-size: 0.8rem;
    }
  }
  .nav-right {
    .search-bar {
      .search-space {
        display: inline-block;
        height: 20px;
        border: unset;
        border-bottom: 1px solid black;
      }
    }
  }
  .nav-right,
  .nav-left {
    width: 20%;
    min-width: 250px;
    .nav-item {
      width: 100%;
      text-align: center;
    }
  }
}
</style>