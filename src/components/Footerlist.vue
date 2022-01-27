<template>
  <div> 
    <span class="ft-list-title">Titolo </span>
    <ul>
      <li>Prova</li>
      <li>Prova</li>
      <li>Prova</li>
      <li>Prova</li>
    </ul>
  </div>
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
  }
  ul{
    list-style-type: none;
  }
</style>