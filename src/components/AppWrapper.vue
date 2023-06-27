<template>
    <div class="fix-button">
        <button>
            <span>Prebuilds</span>
        </button>
        <button>
            <i class="fa-light fa-cart-shopping"></i>
            <span>Buy Now</span>
        </button>
    </div>
    <AppHeader />
    <AppMain />
    <AppFooter/>
  </template>

<script>
import AppHeader from './AppHeader.vue'
import AppMain from './AppMain.vue'
import AppFooter from './AppFooter.vue'

export default {
    name: 'AppWrapper',

    components:{
      AppHeader,
      AppMain,
      AppFooter
    }
}
</script>

<style lang="scss">
    .fix-button{
        display: flex;
        flex-direction: column;
        position: fixed;
        z-index: 2;
        right: 15px;
        top: 150px;
    }

    button{
        border: none;
        border-radius: 5px;
    }
</style>
