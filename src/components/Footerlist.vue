<template>
  <ul> 
    <li class="ft-list-title">Titolo </li>
    <li>Prova</li>
    <li>Prova</li>
    <li>Prova</li>
    <li>Prova</li>
  </ul>
</template>

<script>
export default {
  name: 'Footerlist'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .ft-list-title{
    font-weight: bold;
    padding-bottom: 10px;
  }
  ul{
    list-style-type: none;
    margin-right: 10px;
  }
</style>