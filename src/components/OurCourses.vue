<template>
  <div class="my-bg-banner p-3">
    <div class="container p-5">
      <div class="row">
        <div class="col" v-for="course in OurCourseList" :key="course.title">
          <div class="my-card">
            <img :src="course.CourseImg" :alt="course.title">
            <div class="myhover">
              <h2>{{ course.title}}</h2>
              <p>{{course.info}}</p>
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
          info:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium, sint.",
        },
        {
          CourseImg: "/img/course-intensive-200x200.jpg",
          title: "Pass Plus",
          info:"Lorem, ipsum dolor sit amet consectetur adipisicing elit. Animi, vel sed amet maxime error natus libero id laborum aperiam ipsa.",
        },
        {
          CourseImg: "/img/courses-instructor-200x200.jpg",
          title: "Intensive Course",
          info:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Et id, omnis cum sapiente velit laboriosam.",
        },
        {
          CourseImg: "/img/course-intensive-200x200.jpg",
          title: "Instructors",
          info:"Lorem ipsum dolor sit amet consectetur adipisicing elit. Et id, omnis cum sapiente velit laboriosam.Lorem ipsum dolor sit amet consectetur adipisicing elit. Et id, omnis cum sapiente velit laboriosam.",
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
  position: relative;
  img {
    width: 100%;

  }

  &:hover {
    img{
    display: none;
    }

    .myhover {
      padding: 1rem;
      border: 1px solid black;
      border-radius: 20px;
      display: block;
    }
  }


}


.myhover {
  display: none;
  position: absolute;

  :hover {
    display: block;
  }
}
</style>