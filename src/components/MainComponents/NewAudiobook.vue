<template>
    <div class="fancy-background">
        <div class="wrapper">
            <div class="jumbo">
                <img src="../../assets/img/audible-app-2x-600x628.png" alt="">
                <div>
                    <h1 class="title">New Audiobook</h1>
                    <h2>NO TIME TO READ? NO PROBLEM. LISTEN TO IT</h2>
                    <p>Donec fringilla nunc eu turpis dignissim, at auismod sapien tincidunt. Maecenas eleifend congue cursus.</p>
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

    .fancy-background{
        background-image: url(../../assets/img/banner.jpg);
        background-size: cover;
    }
    .wrapper{
        display: flex;
        width: 60%;
    }

    .jumbo{
        text-align: center;
        display: flex;

        img{
            height: 550px;
            padding-top: 50px;
        }
    }

    h2{
        color: ;
    }
</style>