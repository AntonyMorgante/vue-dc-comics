<template>
<div class="column-wrap">
  <ul v-for="(element,index) in lists" :key=index> 
    <li v-for ="(subelement,index) in element" :key=index>
      {{subelement}}
    </li>
  </ul>
</div>
</template>

<script>
export default {
  name: 'Footerlist',
  data(){
    return{
      lists:[
        ["Dc comics","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum"],
        ["Shop","Lorem Ipsum","Lorem Ipsum"],
        ["Dc","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum"],
        ["Sites","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum","Lorem Ipsum"]
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .column-wrap{
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    height: 300px;
  }

  ul{
    list-style-type: none;
    margin-right: 10px;

    li{
      font-size: 14px;
      color: rgb(180, 161, 161);
    }

    li:first-child{
      font-size: 18px;
      margin-bottom:10px;
      text-transform: uppercase;
      color:white;
    }
  }

</style>