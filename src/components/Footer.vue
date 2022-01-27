<template>
  <div>
    <section class="fst-foot-section">
      <div class="space-around container">
        <Feature />
        <Feature />
        <Feature />
        <Feature />
        <Feature />
      </div>
    </section>
    <section class="snd-foot-section container">
      <Footerlist />
      <Footerlist />
      <Footerlist />
      <Footerlist />
    </section>
    <section class="trd-foot-section">
      <div class="space-between container">
        <button type="button">Sign-up now!</button>
        <div>
          <ul>
            <li>Follow us</li>
            <li> <Social /> </li>
            <li> <Social /> </li>
            <li> <Social /> </li>
            <li> <Social /> </li>
            <li> <Social /> </li>
          </ul>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import Feature from './Feature.vue'
import Footerlist from './Footerlist.vue'
import Social from './Social.vue'

export default {
  name: 'Footer',
  components:{
    Feature,
    Footerlist,
    Social
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .container{
    max-width:1170px;
    margin: auto;
  }
  
  .space-around{
    display:flex;
    justify-content: space-around;
  }

  .fst-foot-section{
    background-color: blue;
    padding: 20px 0;
  }

  .trd-foot-section{
    background-color: rgb(48,48,48);

    .space-between{
      display:flex;
      justify-content: space-between;
      align-items: center;

      ul{
        list-style-type : none;
        color: white;

        li{
          display: inline-block;
          padding: 0 10px;
        }
      }
    }
  }

</style>
