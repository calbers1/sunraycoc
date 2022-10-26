<template>
    <span>
        <div class="HomeBanner">
            <div class="HomeBannerText">
                Welcome!
            </div>
        </div>
    </span>
</template>
	
<script>
export default {
	
}
</script>
	
<style lang="scss" scoped>

@import '../Assets/variables.scss';
	    .HomeBanner{
        width: 100vw;
        margin: 0;
        padding: 0;
        background-image: url('~/Assets/img12.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        height: 80vh;
        display: flex;
        align-items: center;
        justify-content: center;

        @media only screen and (max-width: 992px){
            height: 15rem;

        }

        @media only screen and (max-width: 576px){
            height: 10rem;

        }
    }

    .HomeBannerText{
        color: white;
        font-weight:bold;
        font-size: 6rem;
        @media only screen and (max-width: 992px){
            font-size: 4rem;
        }

        @media only screen and (max-width: 576px){
            font-size: 2rem;
        }
    }
</style>