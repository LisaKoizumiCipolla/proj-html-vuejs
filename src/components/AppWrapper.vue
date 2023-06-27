<template>
    <div class="fix-button">
        <button>
            <div>Prebuilds</div>
        </button>
        <button>
            <i class="fa-solid fa-cart-shopping"></i>
            <div>Buy Now</div>
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

<style lang="scss" scoped>
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

        .fa-cart-shopping{
            transform: scaleX(-1);

        }
    }
</style>
