<template>
    <section id="comics">
        <div class="container">
            <div class="blue-banner">Current series</div>
            <div class="flex-start">
                <Album v-for="(album,index) in albums"
                :img="album.thumb"
                :series="album.series"
                :key="index" />
            </div>
            <div>
                <div class="blue-button">Load more</div>
            </div>
        </div>
    </section>
</template>

<script>
import Album from './Album.vue'
import json from '../../dc-comics.json'

export default {
    name: "Comics",
    components: {
        Album
    },
    data(){
        return{
            albums: json
        }            
    }
}

</script>

<style lang="scss" scoped>
    #comics{
        background-color: rgb(28,28,28);
    }

    .container{
        max-width:1170px;
        margin: auto;
        position: relative;
        top: -15px;

        .blue-banner,
        .blue-button{
            background-color: rgb(2,130,249);
            display: inline-block;
            color:white;
            text-transform: uppercase;
            width:200px;
            height: 35px;
            line-height: 35px;
            text-align: center;
            margin-bottom:50px;
        }

        .blue-button{
            font-size: 15px;
            margin-left:calc(50% - 100px);
            margin-bottom: 20px;
        }

        .flex-start{
            display: flex;
            justify-content: flex-start;
            flex-wrap: wrap;
            color: white;
            font-size: 30px;
        }
    }
</style>