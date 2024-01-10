<script>
export default {
    props: {
        fumetto: Object
    }
}
</script>

<template lang="">
    <div class="card">
        <img :src="fumetto.thumb" alt="">
        {{fumetto.series}}
    </div>
</template>

<style lang="scss" scoped>
    .card{
        color: white;
        width: calc(100% / 6 - 10px);
        margin: 30px 5px;
        height: 300px;

        img{
            height: 300px;
            object-fit: cover;
        }
    }
</style>