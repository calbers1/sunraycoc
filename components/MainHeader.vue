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
	
<style scoped lang="scss">

    @import '../Assets/variables.scss';

	.header{
        width: 100%;
        display: flex;
        align-items: center;
        background-color: $primary-bg;
        max-height: 100px;
        @media only screen and (max-width: 992px){
            height: 3rem;
        }
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
        padding-inline: .5rem;
        color: $primary;
        text-decoration: none !important;
    }
</style>