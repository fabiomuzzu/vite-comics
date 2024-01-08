<script>
export default {
    name: 'AppHeader',
    data(){
        return{
            menu: [
                {
                    link: 'Characters',
                    active: true,
                },
                {
                    link: 'Comics',
                    active: false,
                },
                {
                    link: 'Movies',
                    active: false,
                },
                {
                    link: 'Tv',
                    active: false,
                },
                {
                    link: 'Games',
                    active: false,
                },
                {
                    link: 'Collectibles',
                    active: false,
                },
                {
                    link: 'Videos',
                    active: false,
                },
                {
                    link: 'Fans',
                    active: false,
                },
                {
                    link: 'News',
                    active: false,
                },
                {
                    link: 'Shop',
                    active: false,
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
                <div>
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>
                <div class="row">
                    <div v-for="(object, key) in menu" :class="object.active ? 'active' : ''" class="btn_menu">
                        {{object.link}}
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

    .active{
        color: blue;
    }

    .btn_menu{
        padding: 2px;
    }
</style>