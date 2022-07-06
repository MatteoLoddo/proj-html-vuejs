<template>
<div>
  <div class="container p-0">
    <!-- your first lesson -->
    <div class="d-flex justify-content-between position-relative pt-5 pb-5 ">
      <div class="w-50 pb-5 pt-5">
        <h1>get behind the wheel</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde reiciendis dicta, dolorem corporis quia
          explicabo excepturi! Animi molestias suscipit necessitatibus temporibus ea? Repellendus veniam possimus
          aspernatur sint nostrum, optio quas!</p>
      </div>
      <div class="d-flex flex-column my-card">
        <h3 class="p-3">First lesson Free!</h3>
        <p class="m-0 p-4">when you make a block booking with us your first lesson in <br>included feree</p>
        <div class="d-flex flex-column m-2 align-items-center">
          <input class="m-2 w-75" type="text">
          <input class="m-2 w-75" type="text">
          <input class="m-2 w-75" type="text">
          <input class="m-2 w-75" type="text">
          <button class="btn my-button ">Request a callback</button>
        </div>

      </div>
    </div>
  </div>
    <BannerCallUs class="mt-5"></BannerCallUs>
    <OurCourses></OurCourses>

</div>
</template>

<script>
import OurCourses from '../components/OurCourses.vue'
import BannerCallUs from '../components/BannerCallUs.vue';
export default {
  components: {
    BannerCallUs,OurCourses,
  },
  data() {
    return {

    }
  }
}

</script>

<style lang="scss" scoped>

.my-card {
  box-shadow: 5px 5px 25px rgba(0, 0, 0, 0.3);
  text-align: center;
  border: 1px solid black;
  border-radius: 15px;
  position: absolute;
  right: 5%;
  top: -60px;
  background-color: #fff;

  h3 {
    color: #6B9F5A;
  }

}
</style>
