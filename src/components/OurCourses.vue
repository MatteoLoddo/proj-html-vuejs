<template>
  <div class="my-bg-banner">
    <div class="container p-5">
      <div class="row">
        <div class="col" v-for="course in OurCourseList" :key="course.title">
          <img :src="course.img"  :alt="course.title">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      OurCourseList:[
        {
          img:"course-intensive.jpg",
          title:"Course",
        },
        {
          img:"course-passplus-400x399.jpg",
          title:"Pass Plus",
        },
        {
          img:"course-intensive.jpg",
          title:"Intensive Course",
        },
        {
          img:"courses-instructor.jpg",
          title:"Instructors",
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.my-bg-banner {
  background-image: url(../../public/img/promise-background.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;


}
col{
  img{
    width: 100%
  }
}
</style>