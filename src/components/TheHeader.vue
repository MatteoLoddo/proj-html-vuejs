<template>
  <div class="bg-header  ">
    <TheNavBar :nav-bar-list="NavBarList">
    </TheNavBar>
    <div class="container text-light ptb-10">
      <h1>Drive with Avada</h1>
      <h5>We Offer the finest driving tution money con buy</h5>

    </div>
  </div>
</template>

<script>
import TheNavBar from './TheNavBar.vue'
export default {
  components: {
    TheNavBar
  },
  data() {
    return {
      NavBarList: [
        {
          title: "Home",
          info: "",
        },
        {
          title: "About",
          info: "",
        },
        {
          title: "Prices",
          info: "",
        },
        {
          title: "Courses",
          info: "New",
        },
        {
          title: "Location",
          info: "",
        },
        {
          title: "Blog",
          info: "",
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.bg-header {
  background-image: url(../../public/img/homepage-hero-background.jpg);
  object-fit: contain;
  background-repeat: no-repeat;
  background-position: center;

}

.ptb-10 {
  padding: 10rem 0 10rem 0;
}
</style>
