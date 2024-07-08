<script>
export default{
    name: `AppCardComic`,
    props: {
        details: Object
    }
}
</script>

<template>
    <div>
        <img :src="details.thumb" alt="Fumetto">
        <h3>{{details.series}}</h3>
    </div>
</template>

<style lang="scss" scoped>

    div{
        width: calc(100% / 6 - 20px);
        
        

        img{
        width: 100%;
        aspect-ratio: 1/1;
        }

        h3{
            text-align: left;
            font-weight: lighter;
        }
    }

   
</style>