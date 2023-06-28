<template>
    <div>
        <div class="wrapper">
            <div class="top">
                <div class="titles">
                    <h2 class="title">
                        What The Critics Say
                    </h2>
                    <h3 class="subtitle">TESTIMONIALS FROM AROUND THE WORLD</h3>
                </div>
                
                <button class="green-button">Read All Testimonials</button>
            </div>
            <div class="jumbo">
                <div class="jumbo-main">

                    <div class="img-wrapper">
                        <img class="main-img" src="../../assets/img/testimonial2-2x.jpg" alt="">
                        <div class="text">
                            <h2 class="title">
                                Best Author Of His Generation
                            </h2>
                            <div class="line"></div>
                            <p class="big">This book will change your perspective on life</p>
                            <p>Donec fringilla nunc eu turpis dignissim, at euismod sapien tincidunt. Maecenas eleifend congue cursus. In vitae enim quis sem pharetra.Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.</p>
                            <p>Donec rutrum congue leo eget malesuada. Vivamus suscipit tortor eget felis porttitor volutpat. Nulla quis lorem ut liber. Proin eget tortor risus. Praesent sapien massa, convallis a pellentesque nec, egestas non nisi. Donec rutrum congue leo eget malesuada.</p>
                            <div class="newspaper">
                                <img class="logo" src="../../assets/img/nytimes-logo-white-xsmall.png" alt="">
                                <span class="writer">Justine Kilpatrick,</span>
                                <span class="paper">The New York Times</span>
                            </div>
                        </div>
                    </div>

                </div>
                <div class="article">
                    <div class="card-wrapper">
                        <div class="article-card">
                            <h2 class="card-title title">A True Masterpiece, Bravo!</h2>
                            <p>Nulla quis lorem ut libero malesuada feugiat. Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus. Vivamus suscipit tortor eget felis porttitor volutpat. Nulla quis lorem ut libero malesuada feug at.</p>
                        </div>
                        <div class="newspaper">
                            <img class="logo" src="../../assets/img/theguardian-xsmall.png" alt="">
                            <span class="writer">Gerald Hendley,</span>
                            <span class="paper">The Guardian</span>
                        </div>
                    </div>
                    <div class="card-wrapper">
                        <div class="article-card">
                            <h2 class="card-title title">A Unique View On The World</h2>
                            <p>Donec sollicitudin molestie malesuada. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui. Nulla quis lorem ut libero malesuada feugiat. Vestibulum ac diam sit amet.</p>
                        </div>
                        <div class="newspaper">
                            <img class="logo" src="../../assets/img/theguardian-xsmall.png" alt="">
                            <span class="writer">Mary Maxey,</span>
                            <span class="paper">The Globe And Mail</span>
                        </div>
                    </div>
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


    
    .wrapper{
        width: 70%;
        text-align: initial;
        padding: 80px 0 115px;
    }

    .top{
        display: flex;
        align-items: center;
        justify-content: space-between;

            h2{
                color: black;
                padding-bottom:10px;
            }

            .subtitle{
                color: #49a987;
                padding-bottom: 25px;
            }

            button{
                background-color: #f4b429;
                padding: 10px 45px;
                margin-bottom: 40px;

                    &:hover{
                        background-color: #be8d21;
                    }
            }
    }


    .jumbo{
        width: 100%;
        display: flex;
    }

    .jumbo-main{
        width: 58%;

    .img-wrapper{
        position: relative;
        width: 100%;
        object-fit: cover;
    }

    .main-img{
        border-radius: 0 0 80px 0;
        height: 745px;
        width: 100%;
        object-fit: cover;
    }

    }

    .text{
        position: absolute;
        top: 100px;
        right: 50%;
        transform: translate(50%);
        width: 76%;

        h2{
        color: white;
        }

        .line{
            width: 100%;
            color: #4f4f4f;
            padding: 25px 0;
        }

        p{
            font-size: 1.15rem;
            color: white;
            padding-bottom: 10px;
        }

        .big{
            font-size: 1.3rem;
            padding: 35px 0 10px;
        }
    }

    .newspaper{
        display: flex;
        align-items: center;
        padding-top: 10px;

            .logo{
                height: 100%;
                border-radius: 50%;
                padding-right: 20px;
            }

            span{
                font-weight: 700;
                color: white;
                font-size: 1.1rem;
            }

            .paper{
                color: #49a987;
            }
    }

    .article{
        width: 44%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;

        .writer{
            color: $gray;
        }

        .paper{
            color: black;
            font-weight: 300;

                &:hover{
                    color: $yellow;
                    cursor: pointer;
                }
        }
    }


    .card-wrapper{
        width: 100%;
        margin-left: 60px;
        display: flex;
        flex-direction: column;
    }
    .article-card{
        background-color: $soft_yellow;
        width: 90%;
        padding: 45px 60px 35px;
        text-align: center;
        color: #737373;

        .card-title{
            font-size: 1.5rem;
            color: black;
            padding-bottom: 15px;
        }

        p{
            font-size: 1.15rem;
            line-height: 1.7;
        }
    }


</style>