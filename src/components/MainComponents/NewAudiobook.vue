<template>
    <div class="fancy-background">
        <div class="wrapper">
            <div class="jumbo">
                <img src="../../assets/img/audible-app-2x-600x628.png" alt="">
                <div class="text">
                    <h1 class="title">New Audiobook</h1>
                    <h2>NO TIME TO READ? NO PROBLEM. LISTEN TO IT</h2>
                    <p>Donec fringilla nunc eu turpis dignissim, at auismod sapien tincidunt. Maecenas eleifend congue cursus.</p>
                    <button class="green-button"><i class="fa-brands fa-audible"></i>Buy This On Audible</button>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;

    .fancy-background{
        background-image: url(../../assets/img/banner.jpg);
        background-size: cover;
        background-position-y: 50%;
    }
    .wrapper{
        width: 60%;
    }

    .jumbo{
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        display: flex;

        img{
            height: 600px;
            padding-top: 80px;
        }
    }

    h2{
        color: $yellow;
        font-size: 1.1rem;
        font-weight: 400;
        padding: 25px 0;
    }

    .text{
        text-align: center;
        width: 480px;
        margin-left: 80px;

        p{
            color: $light_gray;
            font-size: 1.15rem;
        }

        img{
            height: 10px;
        }

        i{
            padding-right: 10px;
        }
    }
</style>