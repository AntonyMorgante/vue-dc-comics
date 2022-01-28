<template>
  <div>
    <section class="fst-foot-section">
      <div class="container">
        <Feature />
      </div>
    </section>
    <section class="snd-foot-section">
      <div class ="container">
        <div class="flex-column">
          <Footerlist />
        </div>
      </div>

    </section>
    <section class="trd-foot-section">
      <div class="space-between container">
        <a href="#" class="blue-button">Sign-up Now!</a>
        <div>
          <div class="space-between">
            <span>Follow us</span>
            <div> <Social /> </div>
          </div>
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

  .fst-foot-section{
    background-color: rgb(2,130,249);
    padding: 20px 0;
  }

  .snd-foot-section{
    background-image: url("../assets/footer-bg.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    padding: 20px;
    color: white;

    .flex-column{
      display:flex;
      flex-direction: column;
      flex-wrap: wrap;
      height: 300px;
      align-content: flex-start;
    }
  }

  .trd-foot-section{
    background-color: rgb(48,48,48);

    .blue-button{
      border: solid 1px rgb(2,130,249);
      display: inline-block;
      color:white;
      text-transform: uppercase;
      text-decoration: none;
      width:200px;
      height: 35px;
      line-height: 35px;
      text-align: center;
      margin:10px 0;
    }

    .space-between{
      display:flex;
      justify-content: space-between;
      align-items: center;

      span{
        color:rgb(2,130,249);
        text-transform: uppercase;
      }
    }
  }
  
</style>
