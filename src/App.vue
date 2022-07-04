<template>
  <div id="app">
    <TheHeader></TheHeader>
    <TheMain></TheMain>
    <TheFooter class="bg-footer"></TheFooter>

  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheMain from './components/TheMain.vue'
import TheFooter from './components/TheFooter.vue'


export default {
  name: 'App',
  components: {
    TheHeader,
    TheMain,
    TheFooter,
  }
}
</script>

<style lang="scss">
#app {}

.bg-footer {
  background-image: url(../public/img/testimonial-background.jpg);
  background-position: center;

}
</style>
