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
        font-size: .75rem;
        font-weight: 700;
        color: #4a5259;
        box-shadow: 0 -5px 20px 5px rgba(0,0,0,.15);

        i{
            padding: 17px;
        }

        .fa-cart-shopping{
            transform: scaleX(-1);
            height: 10px;

        }
    }
</style>
