<template>
  <ul>
    <li v-for="(element,index) in socials" :key="index">
      <a :href="element.url">
        <img :src="element.image">
      </a>
    </li>    
  </ul>
</template>

<script>
export default {
  name: 'Social',
  data: function(){
    return{
      socials:[
        {
          name: "Facebook",
          image: require("../assets/footer-facebook.png"),
          url: "#"
        },
        {
          name: "Facebook",
          image: require("../assets/footer-periscope.png"),
          url: "#"
        },
        {
          name: "Facebook",
          image: require("../assets/footer-pinterest.png"),
          url: "#"
        },
        {
          name: "Facebook",
          image: require("../assets/footer-twitter.png"),
          url: "#"
        },
        {
          name: "Facebook",
          image: require("../assets/footer-youtube.png"),
          url: "#"
        }]
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  ul{
    list-style-type : none;
    color: white;

    li{
      display: inline-block;
      padding: 0 10px;
    }
  }
</style>