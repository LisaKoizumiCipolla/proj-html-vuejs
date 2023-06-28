<template>
    <div>
                
        <div class="single-card">
            <img :src="getImage(thumb)">
            <div class="text">
                <h3> {{ title }}</h3>
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
        title : String,
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
            position: relative;
            object-fit: cover ;
        }

        img{
            height: 520px;
            width: 410px;
            border-radius: 0 0 40px 0;
            object-fit: cover;
            object-position: 5%;
        }

        .text{
            text-align: center;
            padding: 20px 25px;
            position: absolute;
            bottom: 0;
            right: 50%;
            transform: translate(50%);
            width: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        h3{
            font-weight: 300;
            font-size: 1.9rem;
            color: white;
            padding-bottom: 20px;
        }

        p{
            padding-top: 20px;
            color: $yellow;
        }

        .line{
            width: 50px;
            border-bottom: 2px solid;
        }
</style>