<template>
  <div class="my-opacity p-3">
    <div class="container d-flex justify-content-between align-items-center  ">
      <div class="">
        <img src="../../public/img/avada-drivers-logo-2x-300x58.png" alt="">
      </div>
      <div class="d-flex p-3">
        <ul class="list-unstyled d-flex mb-0 ">
          <li v-for="items in NavBarList" :key="items.title" class="">
            <a class="p-3 fs-5" href="#">{{ items.title }}</a>
            <span class="info-items" v-if="items.info">{{ items.info }}</span>
          </li>
        </ul>
        <button class="my-button">BOOK NOW</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    NavBarList: Array,

  },
  data() {
    return {

    }
  }
}
</script>


<style lang="scss" scoped>
a {
  text-decoration: none;
  color: #fff;
  font-weight: 700;
  border-bottom: 2px solid transparent;

  &:hover {
    color: #6B9F5A;
    border-bottom: 2px solid #6B9F5A;

  }
}

.my-opacity {
  background-color: rgba(0, 0, 0, 0.5);
}

.info-items {
  color: #fff;
  background-color: #6B9F5A;
  border-radius: 5px;
  padding: 0.2rem;
}
</style>
