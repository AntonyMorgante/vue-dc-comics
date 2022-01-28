<template>
<div class="container">
    <div class="space-between">
        <img src="../assets/dc-logo.png" alt="">
        <ul>
            <li v-for="(element, index) in links" :key="index" :class="{active: isActive}">
                <a href="#">
                    {{element.name}}
                </a>
            </li>
        </ul>
    </div>
</div>
</template>

<script>
export default {
  name: 'Header',
  data: function(){
      return{
          links:[
              {
                  name: "Characters",
                  url: "#",
                  current: false
              },
              {
                  name: "Comics",
                  url: "#",
                  current: false
              },
              {
                  name: "Movies",
                  url: "#",
                  current: false
              },
              {
                  name: "Tv",
                  url: "#",
                  current: false
              },
              {
                  name: "Games",
                  url: "#",
                  current: false
              },
              {
                  name: "Collectibles",
                  url: "#",
                  current: false
              },
              {
                  name: "Videos",
                  url: "#",
                  current: false
              },
              {
                  name: "Fans",
                  url: "#",
                  current: false
              },
              {
                  name: "News",
                  url: "#",
                  current: false
              },
              {
                  name: "Shop",
                  url: "#",
                  current: false
              }
          ]
      }
  }
}
</script>

<style scoped lang="scss">
.container{
    max-width:1170px;
    margin: 0 auto;
    padding: 10px;

    .space-between {
        display: flex;
        justify-content: space-between;
        align-items: center;

        ul{
            list-style-type: none;

            li{
                display:inline-block;
                padding: 0 10px;
                text-transform: uppercase;

                a{
                    text-decoration: none;
                    color: black;
                }
            }
        }
    }
}

</style>