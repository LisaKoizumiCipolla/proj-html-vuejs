<template>
    <nav>
        <img class="logo" src="../assets/img/author-logo-round-small.png" alt="">
        <ul>
            <li class="colour">Home</li>
            <li>About Me</li>
            <li>Testimonials</li>
            <li>My Blog</li>
            <li>Meetups</li>
            <li>Shop <span><i class="fa-solid fa-chevron-down fa-2xs"></i></span></li>
            <li>Contact Me</li>
            <li><i class="fa-solid fa-cart-shopping "></i></li>
        </ul>
    </nav>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

nav{
    padding: 0px 87px 0;
    display: flex;
    justify-content: space-between;
}

.logo{
    height: 140px;
}

ul{
    margin-bottom: 25px;
    padding-right: 18px;
    display: flex;
}

li{
    margin-left: 45px;
    margin-bottom: 7px;
    font-weight: 400;
    height: 50px;
    padding-top: 50px;


    &:hover{
        color: $yellow;
        border-top: 5px solid $yellow;
        padding-top: 45px;
        cursor: pointer;
    }

    .fa-chevron-down{
        vertical-align: 0.1em;
    }

    .fa-cart-shopping{
        font-size: .8rem;
    }

    span{
        padding-left: 3px;
    }
}

.colour{
    color: $yellow;
        border-top: 5px solid $yellow;
        padding-top: 45px;
}
    
</style>