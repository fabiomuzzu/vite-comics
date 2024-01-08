<script>
export default {
    name: 'AppHeader',
    data(){
        return{
            menu: [
                {
                    link: 'Characters'
                },
                {
                    link: 'Comics'
                },
                {
                    link: 'Movies'
                },
                {
                    link: 'Tv'
                },
                {
                    link: 'Games'
                },
                {
                    link: 'Collectibles'
                },
                {
                    link: 'Videos'
                },
                {
                    link: 'Fans'
                },
                {
                    link: 'News'
                },
                {
                    link: 'Shop'
                }
            ]
        }
    }
}
</script>

<template lang="">
    <header>
        <div class="container">
            <div class="row">
                <div class="mw-1200" >
                    <div class="col">
                        <div class="logo_container">
                            <img src="../assets/img/dc-logo.png" alt="">
                        </div>
                    </div>
                    <div class="col">
                        <div v-for="(link, index) in menu" :key="index">

                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<style lang="scss">
    header{
        background-color: white;
    }
</style>