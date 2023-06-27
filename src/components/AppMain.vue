<template>
    <div>
        <MoreAbout />
        <BuyLink />
        <NewAudiobook />
    </div>
</template>

<script>
import MoreAbout from "./MainComponents/MoreAbout.vue"
import BuyLink from "./MainComponents/BuyLink.vue"
import NewAudiobook from "./MainComponents/NewAudiobook.vue"


export default {

    components: {
        MoreAbout,
        BuyLink,
        NewAudiobook,
    } 
}
</script>
<style lang="scss" scoped>
</style>