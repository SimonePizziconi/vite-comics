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
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="Fumetto">
        <h3>Action comic</h3>
    </div>
</template>

<style lang="scss" scoped>

    div{
        width: calc(100% / 6);

        img{
        width: 100%;
        }

        h3{
            text-align: center;
        }
    }

   
</style>