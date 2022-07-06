<template>
  <div class="my-bg-banner">
    <div class="container p-5">
      <div class="row">
        <div class="col" v-for="course in OurCourseList" :key="course.title">
          <div class="my-card">
            <img :src="course.CourseImg" :alt="course.title">
            <div class="myhover">
              <h2>{{ course.title }}</h2>
              <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Minus nesciunt repellat quia iure reiciendis
                rem, consectetur voluptatem earum. Recusandae, provident.</p>
              <button class="my-button">course information</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      OurCourseList: [
        {
          CourseImg: "/img/courses-passplus-200x200.jpg",
          title: "Course",
        },
        {
          CourseImg: "/img/course-intensive-200x200.jpg",
          title: "Pass Plus",
        },
        {
          CourseImg: "/img/courses-instructor-200x200.jpg",
          title: "Intensive Course",
        },
        {
          CourseImg: "/img/course-intensive-200x200.jpg",
          title: "Instructors",
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

.col {
  img {
    width: 100%;

  }

  &:hover {
    img{
    display: none;
    }

    .myhover {
      display: block;
    }
  }


}


.myhover {
  display: none;

  :hover {
    display: block;
  }
}
</style>