<script>
export default {
    name: 'AppHeader',
    data(){
        return{
            menu: [
                {
                    link: 'Characters',
                    active: false,
                },
                {
                    link: 'Comics',
                    active: true,
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
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>
                <div class="menu">
                    <ul>
                        <li v-for="(object, key) in menu"><a href="" :class="object.active ? 'active' : ''" class="btn_menu">{{object.link}}</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>

<style lang="scss">
@use '../styles/generals.scss' as *;
@use '../styles/partials/variables' as *;
    .menu{
        display: flex;
        align-items: center;
    }

    ul{
        display: flex;
        list-style-type: none;        
        li{
            margin: 0 10px;
            a{
                text-transform: uppercase;
                color: black;
                font-weight: 700;
                position: relative;

            }
        }
    }
    
    .logo{
        img{
            width: 80px;
        }
    }
    
    .row{
        padding: 10px 0;
    }
    
    header{
        background-color: white;
    }
    
    .active{
        color: $primary_color;
        &::after{
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 2px;
            background-color: $primary_color;
        }
    }
    
    .btn_menu{
        padding: 2px;
    }
</style>