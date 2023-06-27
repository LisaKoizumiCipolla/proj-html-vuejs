<template>

    <div class="background">
        <div class="wrapper">
            <h1 class="title">Upcoming Events</h1>
            <h2 class="subtitle">MEET THE AUTHOR  IN PERSON</h2>
            <div class="cards-wrapper">
                <EventCards v-for="event in eventList"
                    :thumb="event.thumb"
                    :event="event.event"
                    :description="event.description"
                
                />
            </div>
        </div>
    </div>
</template>
<script>
import EventCards from './EventCards.vue';

export default {

    components: { 
        EventCards 
    },
    data(){
        return{
            eventList:[
                {
                    thumb: 'event-05-600x359.jpg',
                    event: 'Chicago Book Signing',
                    description: 'Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a nulla.',
                },
                {
                    thumb: 'event-04-600x359.jpg',
                    event: 'Meet & Greet With Amanda',
                    description: 'Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Praesent sapien massa, convallis a pellentesque nec, egestas.',
                },
                {
                    thumb: 'event-07-600x359.jpg',
                    event: 'Open Book: Dialogues',
                    description: 'Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a nulla.',
                },
            ],
        }
    }

}
</script>
<style lang="scss" scoped>
@use '../../styles/partials/variables' as *;

    .background{
        background-color: $soft_yellow;
        padding: 70px;
    }

    .wrapper{
        width: 85%;
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
        padding: 10px 0 20px;
        color: $yellow;
    }


</style>