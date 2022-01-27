<template>
<div class="content">
  <div class="container">
    Content here
  </div>
</div>

</template>

<script>
export default {
  name: 'Main'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .content{
    background-color: rgb(28,28,28);

    .container{
      max-width:1170px;
      margin: auto;
      color: white;
      padding: 100px;
      font-size: 30px;
    }
  }
</style>
