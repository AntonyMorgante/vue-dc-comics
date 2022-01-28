<template>
    <div class="comic">
        <img :src="img" alt="">
        <p>{{ series }}</p>
    </div>
</template>

<script>
export default {
    name: "Album",
    props:{
        img: String,
        series: String
    }
}
</script>

<style lang="scss" scoped>
    .comic{
        flex-basis: calc(100% / 6);
        text-align: start;
        padding-bottom:20px;

        img{
            width:90%;
        }

        p{
            width: 90%;
            font-size: 12px;
            text-transform: uppercase;
        }
    }
</style>