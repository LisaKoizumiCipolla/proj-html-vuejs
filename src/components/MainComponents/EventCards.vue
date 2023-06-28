<template>
    <div>
                
        <div class="single-card">
            <div class="img">
                <img :src="getImage(thumb)">
            </div>
            <div class="text">
                <h3> {{ event }}</h3>
                <div class="line"></div>
                <p class="gray-text"> {{ description }}</p>
            </div>
        </div> 

    </div>
</template>
<script>
export default {
    props: {
        thumb : String,
        event : String,
        description : String
    },
    methods : {
        getImage : function(img){
            return new URL(`../../assets/img/${img}`, import.meta.url).href;
        }
    }
}
</script>
<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;
        .single-card{
            width: 100%;
            padding: 25px;
            transition: transform 0.5s;

            &:hover{
                filter: saturate(50%);
            }
        }
    
        img{
            width: 100%;
        }

        .text{
            background-color: white;
            padding: 40px 35px;
        }

        h3{
            font-weight: 300;
            font-size: 1.6rem;
            padding-bottom: 20px;

                    &:hover{
                        color: $yellow;
                        cursor: pointer;
                    }
        }

        p{
            padding-top: 25px;
        }

        .line{
            width: 100%;
            border-bottom: 1px solid;
        }
</style>