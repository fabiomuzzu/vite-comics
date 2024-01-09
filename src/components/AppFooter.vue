<script>
export default {
    name: 'AppFooter',
    data(){
        return{
           
        }
    }
}
</script>

<template lang="">
    <footer>
        <div class="top_footer">
            <div class="container">
                <div class="top-footer-inner">
                    <div class='top-footer-menu'>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li><a href="">Characters</a></li>
                            <li><a href="">Comics</a></li>
                            <li><a href="">Movies</a></li>
                            <li><a href="">Tv</a></li>
                            <li><a href="">Games</a></li>
                            <li><a href="">Videos</a></li>
                            <li><a href="">News</a></li>
                        </ul>
                    </div>
                    <div class='top-footer-menu'>

                    </div>
                    <div class='top-footer-menu'>

                    </div>
                </div>
            </div>
        </div>
        <div class="bottom_footer">

        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.top_footer{
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;

    .top-footer-inner{
        background-image: url(../assets/img/dc-logo-bg.png);
        background-position: right;
        background-repeat: no-repeat;
        display: flex;
    }
}

h3{
    color: white;
}
</style>