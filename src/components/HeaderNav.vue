<template>
    <nav>
        <img class="logo" src="../assets/img/author-logo-round-small.png" alt="">
        <ul>
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
    padding: 4px 87px 0;
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
    align-items: center;
}

li{
    padding-left: 45px;
    padding-bottom: 7px;
    font-weight: 400;

    &:hover{
        color: #F4B429;
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
    
</style>