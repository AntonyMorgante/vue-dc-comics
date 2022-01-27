<template>
<div class="container">
    <div class="space-between">
        <img src="../assets/dc-logo.png" alt="">
        <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>Tv</li>
            <li>Games</li>
            <li>Collectibles</li>
            <li>Videos</li>
            <li>Fans</li>
            <li>News</li>
            <li>Shop</li>
        </ul>
    </div>
</div>
</template>

<script>
export default {
  name: 'Header'
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
            }
        }
    }
}

</style>