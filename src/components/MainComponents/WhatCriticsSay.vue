<template>
    <div>
        <div class="wrapper">
            <div class="jumbo">
                <div class="jumbo-main">
                    <h2 class="title">
                        What The Critics Say
                    </h2>
                    <h3>TESTIMONIALS FROM AROUND THE WORLD</h3>
                    <div>
                        <div class="critic">
                            <div class="background"></div>
                        </div>
                        <div class="text">
                            <h2 class="title">
                                Best Author Of His Generation
                            </h2>
                            <div></div>
                            <h4></h4>
                            <p></p>
                        </div>
                    </div>
                </div>
                <div class="cards"></div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>

    .wrapper{
        width: 70%;
    }

    .jumbo{
        width: 100%;
    }

    .jumbo-main{
        width: 65%;
    }

    .critic{
        position: relative;
        width: 100%;
    }
    .background{
        background-image: url(../../assets/img/testimonial2-2x.jpg);
        border-radius: 0 0 80px 0;
        height: 800px;
        background-size: cover;
    }

</style>