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
                        <h3>SHOP</h3>
                        <ul>
                            <li><a href="">Shop DC</a></li>
                            <li><a href="">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <div class='top-footer-menu'>
                        <h3>DC</h3>
                        <ul>
                            <li><a href="">Terms Of Use</a></li>
                            <li><a href="">Privacy policy (New)</a></li>
                            <li><a href="">Ad Choices</a></li>
                            <li><a href="">Advertising</a></li>
                            <li><a href="">Jobs</a></li>
                            <li><a href="">Subscriptions</a></li>
                            <li><a href="">Talent Workshops</a></li>
                            <li><a href="">CPSC Certificates</a></li>
                            <li><a href="">Ratings</a></li>
                            <li><a href="">Shop Help</a></li>
                            <li><a href="">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class='top-footer-menu'>
                        <h3>SITES</h3>
                        <ul>
                            <li><a href="">DC</a></li>
                            <li><a href="">MAD Magazine</a></li>
                            <li><a href="">DC Kids</a></li>
                            <li><a href="">DC Universe</a></li>
                            <li><a href="">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="bottom_footer">
            <div class="container">
                <div class="row">
                    <div class="bottom-footer-menu">
                        <button class="button-primary">SIGN-UP NOW!</button>
                    </div>
                    <div class="bottom-footer-menu">
                        <div class="links">
                            <h3>FOLLOW US</h3>
                            <a href="">
                            <img class="social_logo" src="../assets/img/footer-facebook.png" alt="">
                            </a>
                            <a href="">
                            <img class="social_logo" src="../assets/img/footer-twitter.png" alt="">
                            </a>
                            <a href="">
                            <img class="social_logo" src="../assets/img/footer-youtube.png" alt="">
                            </a>
                            <a href="">
                            <img class="social_logo" src="../assets/img/footer-pinterest.png" alt="">
                            </a>
                            <a href="">
                            <img class="social_logo" src="../assets/img/footer-periscope.png" alt="">
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.bottom_footer{
    background-color: rgb(72, 72, 72);
    .bottom-footer-menu{
        margin: 0 30px;
        padding: 10px 0;

        .social_logo{
            padding: 0 8px;
        }

        .links{
            display: flex;
            align-items: center;
            h3{
                color: $primary_color;
                margin-right: 10px;
            }
        }
    }
    
    .button-primary {
        padding: 10px 10px;
        border: 2px solid $primary_color;
        color: white;
        background-color: transparent;
        cursor: pointer;
    }
}

footer{
    min-width: 980px;
}
.top_footer{
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;

    .top-footer-inner{
        background-image: url(../assets/img/dc-logo-bg.png);
        background-position: right;
        background-repeat: no-repeat;
        display: flex;
    }

    .top-footer-menu{
        h3{
            color: white;
            margin: 0 30px;
        }
        padding: 50px 0;
        ul {
            list-style-type: none;
            padding: 15px 0;
            margin: 0 30px;
            li{
                text-decoration: none;
                padding: 5px 0;
                a{
                    color: gray;
                }
            }
        }
    }
}

</style>