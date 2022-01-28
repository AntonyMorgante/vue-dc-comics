<template>
  <div class="space-around">
    <div v-for="(element,index) in features" :key="index" class="ft-flex-start">
      <img :src="element.image">
      <span>{{element.name}}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Feature',
  data: function(){
    return{
      features: [
        {
          name:"digital comics",
          image: require("../assets/buy-comics-digital-comics.png")
        },
        {
          name:"merchandise",
          image:require("../assets/buy-comics-merchandise.png")
        },
        {
          name:"shop locator",
          image:require("../assets/buy-comics-shop-locator.png")
        },
        {
          name:"subscriptions",
          image:require("../assets/buy-comics-subscriptions.png")
        },
        {
          name:"power-visa",
          image:require("../assets/buy-dc-power-visa.svg")
        },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
  .space-around{
    display:flex;
    justify-content: space-around;
  }

  .ft-flex-start{
    display:flex;
    justify-content: flex-start;
    align-items: center;
    color: white;
    flex-basis: 20%;
    text-transform: uppercase;
    align-items: center;

    img{
      height: 70px;
      max-width: 30%;
      margin-right: 15px;
    }

    span{
      font-size: 12px;
      width:50%
    }
  }
</style>