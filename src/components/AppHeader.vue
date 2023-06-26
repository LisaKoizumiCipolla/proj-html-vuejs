<template>
    <header>
        <div class="header">
            <div class=".header-footer-wrapper">
                <HeaderNav />
            </div>
        </div>
    </header>
</template>

<script>
import HeaderNav from './HeaderNav.vue'

export default {
    components : {
        HeaderNav
    }
}
</script>

<style lang="scss" scoped>
    
    .header{
        background-color: black;
        background-image: url(../assets/img/hero-07-2x.jpg);
        background-size: cover;
        background-position: 50%;
        height: 100vh;
        color: white;
    }
</style>