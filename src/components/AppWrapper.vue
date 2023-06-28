<template>
    <div class="fix-button">
        <button>
            <i class="fa-solid fa-folder-open fa-lg"></i>
            <div>Prebuilds</div>
        </button>
        <button>
            <i class="fa-solid fa-cart-shopping fa-xl"></i>
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
        background-color: white;
        margin-bottom: 10px;
        padding: 5px;
        font-size: .8rem;
        font-weight: 600;
        color: #4a5259;

        i{
            padding: 15px 0;
        }

        .fa-cart-shopping{
            transform: scaleX(-1);
            height: 10px;

        }
    }
</style>
