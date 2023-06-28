<template>

    <div class="background">
        <div class="wrapper">
            <h1 class="title">Dig A Little Deeper Into Damon Vaughn</h1>
            <h2 class="subtitle">FIND OUT MORE ABOUT THE AUTHOR HIMSELF</h2>
            <div class="cards-wrapper">
                <SpadeElement v-for="event in eventList"
                    :thumb="event.thumb"
                    :title="event.title"
                    :description="event.description"

                />
            </div>
        </div>
    </div>
</template>
<script>
import SpadeElement from './SpadeElement.vue';

export default {

    components: { 
        SpadeElement 
    },
    data(){
        return{
            eventList:[
                {
                    thumb: 'spade1.jpg',
                    title: 'About Me',
                    description: 'Vestibulum ante ipsum primis',
                },
                {
                    thumb: 'spade2.jpg',
                    title: 'My Latest Book',
                    description: 'Vestibulum ante ipsum primis',
                },
                {
                    thumb: 'spade3.jpg',
                    title: 'Book Signing',
                    description: 'Vestibulum ante ipsum primis',
                },
            ],
        }
    }

}
</script>
<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;

    .background{
        background-color: white;
        padding: 70px;
    }

    .wrapper{
        width: 75%;
    }

    .cards-wrapper{
        display: flex;
        justify-content: space-between;
        width: 100%;
    }

    .title{
        color: black;
    }

    h2{
        padding: 10px 0 50px;
        color: #49a987;;
    }


</style>