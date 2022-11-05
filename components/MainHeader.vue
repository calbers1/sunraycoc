<template>
    <span class="header">
        <span class="header-logo col-2">
            <img src="../Assets/logo-main.png"/>
        </span>

        <span class="header-menu col-12 col-lg-8">
            <NuxtLink to="/">Home</NuxtLink>
            <NuxtLink to="/About">About</NuxtLink>
            <NuxtLink to="/Staff">Staff</NuxtLink>
            <NuxtLink to="/Media">Media</NuxtLink>
            <NuxtLink to="/Contact">Contact</NuxtLink>
        </span>
        
    </span>
</template>
	
<script>
export default {
	
}
</script>
	
<style lang="scss">


    @import '../Assets/variables.scss';

    .main-content{
        background-color: $secondary-bg;
        color: $primary;
        padding: 0 1rem;
    }
    $theme-colors: (
        "primary": $primary,
        "secondary": $secondary,
    );
	.header{
        width: 100%;
        display: flex;
        align-items: center;
        background-color: $primary-bg;
        max-height: 100px;
        @media only screen and (max-width: 992px){
            height: 3rem;
        }
        border-bottom: 2px solid $primary;
    }

    .header-logo{
        padding: 8px;

        @media only screen and (max-width: 992px){
            display: none;
        }
    }

    .header-logo > img{
        width: 250px;
    }

    .header-menu{
        display: flex;
        width: 100%;
        justify-content: center;
    }

    .header-menu a{
        padding-inline: .75rem;
        font-weight: bold;
        color: $primary;
        text-decoration: none !important;
    }
</style>