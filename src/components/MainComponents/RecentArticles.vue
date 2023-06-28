<template>
    <div class="section">
        <div class="wrapper">
            <div class="top">
                <div class="titles">
                    <h2 class="title">
                        Recent Articles
                    </h2>
                    <h3 class="subtitle">READ THE LATEST ENTRIES</h3>
                </div>
                
                <button class="green-button">All Articles</button>
            </div>
            <div class="jumbo">
                <div class="jumbo-main">

                    <div class="img-wrapper">
                        <img class="main-img" src="../../assets/img/20-Tips-600x353.jpg" alt="">
                        <div class="text">
                            <p class="big">20 Creativity Tips</p>
                            <p class="by">By <span>admin</span> | October 24th, 2019 | Categories: <span>Event, Tips & Tricks</span></p>
                            <p>Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet. </p>
                            
                        </div>
                    </div>

                </div>
                <div class="article">
                    <div class="card-wrapper">
                        
                            <img src="../../assets/img/thumb-13-2x-700x441.jpg" alt="">
                        
                        <div class="info">
                            <p class="big">What's On Your Booklist</p>
                            <p class="by">By <span>admin</span> | October 24th, 2019 </p>
                        </div>
                    </div>
                    <div class="card-wrapper">
                        
                            <img src="../../assets/img/thumb-08-2x-700x441.jpg" alt="">
                        
                        <div class="info">
                            <p class="big">Istanbul Travel Guide</p>
                            <p class="by">By <span>admin</span> | October 24th, 2019 </p>
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

    .section{
        background-color: #fef7e9;
    }

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
                padding: 10px 80px;
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
        width: 65%;

    .img-wrapper{
        width: 100%;
        object-fit: cover;
        background-color: white;
        padding: 50px;
    }

    .main-img{
        width: 100%;
        object-fit: contain;
    }

    }

    .text{
        top: 100px;
        width: 100%;
        padding: 40px 0 0 20px;


        p{
            font-size: 1.15rem;
            color: $gray;
            margin-bottom: 0;
        }

        .big{
            font-size: 1.65rem;
            color: black;
        }

        .by{
            font-size: .9rem;
            padding-bottom: 15px;
        }
    }

    span{
        color: black;

        &:hover{
            color: $yellow;
            cursor: pointer;
        }
    }


    .article{
        width: 35%;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }


    .card-wrapper{
        width: 410px;
        height: 50%;
        margin-left: 47px;
        display: flex;
        flex-direction: column;
        background-color: white;
        position: relative;
        object-fit: cover;
        padding: 40px 40px 20px 40px;

        img{
            object-fit: cover;
            width: 100%;
            height: 100%;
        }
    }

    .info{
        position: absolute;
        background-color: white;
        bottom: 0;
        width: 82%;
        padding: 5px 0 30px 30px;

        .big{
            font-size: 1.6rem;
            padding-top: 25px;
            margin-bottom: 0;
        }

        .by{
            font-size: .8rem;
        }
    }
    


</style>