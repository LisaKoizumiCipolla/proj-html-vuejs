<template>
    <body class="main-font">
                <MoreAbout />
                <BuyLink />
                <NewAudiobook />
                <WhatCriticsSay />
                <UpcomingEvents />
                <SubscribeTo />
                <DigDeeper />
                <RecentArticles />
    </body>
</template>

<script>
import MoreAbout from "./MainComponents/MoreAbout.vue"
import BuyLink from "./MainComponents/BuyLink.vue"
import NewAudiobook from "./MainComponents/NewAudiobook.vue"
import WhatCriticsSay from "./MainComponents/WhatCriticsSay.vue";
import UpcomingEvents from "./MainComponents/UpcomingEvents.vue";
import SubscribeTo from "./MainComponents/SubscribeTo.vue";
import DigDeeper from "./MainComponents/DigDeeper.vue";
import RecentArticles from "./MainComponents/RecentArticles.vue";


export default {

    components: {
    MoreAbout,
    BuyLink,
    NewAudiobook,
    WhatCriticsSay,
    UpcomingEvents,
    SubscribeTo,
    DigDeeper,
    RecentArticles
} 
}
</script>
<style lang="scss" scoped>
</style>