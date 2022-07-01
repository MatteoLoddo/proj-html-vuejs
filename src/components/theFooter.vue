<template>
  <div class="">
    <div class="container">
      <div class="row">
        <div class="col">
          <img src="../../public/img/avada-drivers-logo-2x-200x39.png" alt="">
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni id asperiores voluptate eveniet eius minima
            veritatis praesentium nostrum soluta vel dolore error quos officiis modi, et at aperiam esse eos.</p>
        </div>

        <div v-for="items in FooterList" :key="items.title" class="col">
          <ul>{{items.title}}
            <li v-for="object in items.listObjects" :key="object.text">{{object.text}}
            </li>
          </ul>
        </div>
      </div>
      <div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {

  },
  data() {
    return {
      FooterList: [
        {
          title: "contact details",
          listObjects: [
            {
              img:"",
              text:"12345 North Main Street New York, NY 55555555"
            },
            {
              img:"",
              text:"1.800.556.6789"
            },
            {
              img:"",
              text:"Info@your-domain.com"
            },
            {
              img:"",
              text:"Theme-fusion.com"
            }
          ]
        },
        {
          title:"Courses",
          img:"",
          listObjects:[
            {
              text:"Pass Plus"
            },
            {
              text:"Intensive Course"
            },
            {
              text:"Automatic"
            },
            {
              text:"Instructor Training"
            },
          ]
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
</style>
