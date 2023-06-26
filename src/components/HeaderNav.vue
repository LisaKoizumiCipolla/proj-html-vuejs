<template>
    <nav class="d-flex justify-content-between">
        <img class="logo" src="../assets/img/author-logo-round-small.png" alt="">
        <ul class="d-flex align-items-center">
            <li>Home</li>
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

nav{
    padding: 0 78px;
    
    font-family: 'DM Sans', sans-serif;
}

.logo{
    height: 140px;
}

li{
    padding-left: 45px;
    padding-bottom: 7px;
    font-weight: 400;

    &:hover{
        color: #F4B429;
    }

    .fa-cart-shopping{
        font-size: .8rem;
    }

    span{
        padding-left: 3px;
    }
}
    
</style>