<template>
    <div class="background">
        <div class="wrapper">
            <div class="subscribe">
                <h1 class="title">Subscribe To My Newsletter</h1>
                <h2 class="subtitle">BE NOTIFIED ABOUT BOOK SIGNING TOUR DATES</h2>
                <input type="text"><button class="green-button">Subscribe</button>
                <p class="gray-text">Donec fringilla nunc eu turpis dignissim, at euismod spien dicidunt.</p>
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
    .background{
        background-image: url(../../assets/img/banner-2.jpg);
        background-size: cover;
        height: 572px;
    }

    .wrapper{
        display: flex;
        align-items: center;
        justify-content: center;
    }

    h1{
        padding: 0px 50px;
    }


    .subscribe{
        text-align: center;
        width: 500px;
        padding-top: 90px;
    }

    h2{
        color: $yellow;
        padding: 30px 0 10px;
    }

    input{
        height: 30px;
    }

    p{
        color: $light-gray;
        padding-top: 35px;
    }

    button{
        margin-left: 20px;
        font-size: 1.1rem;
        padding: 13px 55px;
    }
</style>