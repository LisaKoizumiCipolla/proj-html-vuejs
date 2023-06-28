<template>
    <footer class="main-font">
        <div class="background">
            <div class="header-footer-wrapper">
                <div class="contacts-logo">
                    <img src="../assets/img/author-logo-round-200x205.png" alt="">
                    <div class="contacts">
                        <div class="section">
                            <h2 class="title">ABOUT ME</h2>
                            <p>Vivamus suscipit tortor <span class="bold">eget felis porttitor</span> volutpat. Nulla quis lorem ut libero malesuada feugiat. Vivamus suscipit tortor eget felis porttitor volutpat.</p>
                        </div>
                        <div class="section">
                            <h2 class="title">USEFUL LINKS</h2>
                            <ul>
                                <li v-for="link in links">
                                    <i class="fa-solid fa-chevron-right fa-2xs"></i> {{ link }}
                                </li>
                            </ul>
                        </div>
                        <div class="section">
                            <h2 class="title">CONTACT INFO</h2>
                                <div class="contact-info">
                                    <div>63 E. Studebaker Street Bolingbrook, IL 60440</div>
                                    <div>Phone: (800) 000-0000</div>
                                    <div>Mobile: (800) 000-0000</div>
                                    <div>Email: <span class="colour">info@your-company.com</span></div>
                                    <div class="social">
                                        <i class="fa-brands fa-facebook-f"></i>
                                        <i class="fa-brands fa-twitter"></i>
                                        <i class="fa-brands fa-instagram"></i>
                                        <i class="fa-brands fa-youtube"></i>
                                        <i class="fa-brands fa-linkedin-in"></i>
                                    </div>
                                </div>
                        </div>
                    </div>
                </div>
                <div class="credits"><i class="fa-regular fa-copyright fa-xs"></i> Copyright 2012 - 2023 | Avada Theme by <span class="gray">ThemeFusion</span> | All Rights Reserved | Powered by <span class="gray">WordPress</span></div>
            </div>
        </div>
    </footer>
</template>
<script>
export default {

    data(){
        return{
            links : ["Latest Books", "Upcoming Events", "Recent ARticles", "Business Enquiries", "Visit My Foundation"]
        }
    }
    
}
</script>
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

    .background{
        background-image: url(../assets/img/footer-3.jpg);
        background-size: cover;
        height: 520px;
    }

    .header-footer-wrapper{
        padding: 120px 0 55px;
    }

    img{
        height: 100%;
        margin-right: 100px;
    }

    .contacts-logo{
        display: flex;
    }

    .contacts{
        width: 70vw;
        display: flex;
    }

    .section{
            width: calc( 100% / 3);
            color: #cccccc;

            .title{
                font-size: 1.25rem;
                padding-bottom: 20px;
            }

            p{
                font-size: 1.05rem;
                padding-right: 150px;
                font-weight: 300;
                line-height: 1.8rem;
            }

            .bold{
                font-weight: 700;
            }
        }

        .colour{
            &:hover{
                color: $yellow
            }
        }

        .contact-info div{
            padding-bottom: 15px;
        }

        .contact-info{

            .social{
                padding-top: 20px;
            }

            i{
                padding: 0 20px 0 0;

                &:hover{
                    color: white;
                }
            }
        }

        ul{
            padding-left: 10px;

            li{
                padding-bottom: 15px;

                &:hover{
                    cursor: pointer;
                    color : $yellow
                }
            }
        }
        .fa-chevron-right{
            color: white;
            padding-right: 15px;
        }

        .credits{
            text-align: center;
            color: white;
            padding-top: 50px;
            font-size: .9rem;

            .gray{
                color: $light_gray;

                &:hover{
                    color: $yellow;
                    cursor: pointer;
                }
            }
        }
</style>