<template>
    <header>
        <div class="header">
            <div class=".header-footer-wrapper">
                <HeaderNav />
                <div class="jumbo">
                    <h1 class="sign">Damon Vaughn</h1>
                    <p class="title article">Best-Selling Author And The Most Influential Public Intellectual In The Western World Right Now.</p>
                    <span>- The New York Times</span>
                </div>
                <div class="buy">
                    <div class="buy-main">
                        <img src="../assets/img/book-widget.webp" alt="">
                        <div class="text">
                            <h2 class="title">Latest Book Release</h2>
                            <h3 class="title">D. VAUGHN AUTOBIOGRAPHY</h3>
                            <p>Donec fringilla nunc eu turpis dignissim, at euismod sapien tincidunt. Maecenas eleifend congue cursus.
                            </p>
                        </div>
                    </div>
                    <div class="buttons">
                        <button><i class="fa-brands fa-amazon"></i> Buy On Amazon</button>
                        <button><i class="fa-brands fa-apple"></i> Buy On App Store</button>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
import HeaderNav from './HeaderNav.vue'

export default {
    components : {
        HeaderNav
    }
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
    
    header{
        position: relative;
    }

    .buy{
        background-color: white;
        position: absolute;
        right: 0;
        bottom: 0;
        padding: 60px 60px 40px;

        h2{
            color: black;
        }
    }

    .buy-main{
        display: flex;
    }

    .text{
        width: 330px;

        h2{
            font-size: 2rem;
        }

        h3{
            color: $yellow;
            font-size: 1rem;
        }

        p{
            color: $gray;
            font-size: 1rem;
        }
    }

    .buttons{
        display: flex;
        justify-content: space-between;
        padding: 10px 0 7px;
    }

    button{
        border: 1px solid #49A987;
        border-radius: 5px;
        padding: 10px 75px;
        background-color: #f4faf8;
        font-size: .9rem;
    }

    i{
        padding-right: 5px;
    }
    .header{
        background-image: linear-gradient(rgba(200, 151, 151, 0.05), rgba(0, 0, 0, 0.80)), url(../assets/img/hero-07-2x.jpg);
        background-size: cover;
        background-position: 50%;
        height: 100vh;
        color: white;
        font-family: 'DM Sans', sans-serif;
    }

    .jumbo{
        width: 60%;
        padding: 190px 0 0 230px;
        font-stretch: ultra-expanded;
        letter-spacing: 0.04em;
    }

    .article{
        padding-top: 8px;
        font-size: 3.0rem;
        line-height: 64px;
        margin-bottom: 38px;
    }

    span{
        font-size: 1.45rem;
        color: $light_gray;
    }

</style>