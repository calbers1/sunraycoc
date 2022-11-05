<template>
    <span>
        <div class="HomeBanner">
            <div class="HomeBannerText">
                Welcome to Sunray!
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
        background-image: url('~/Assets/img14.jpg');
        width: 100%;
        margin: 0;
        padding: 0;
        background-size: cover;
        background-position: center bottom;
        background-repeat: no-repeat;
        height: 75vh;
        display: flex;
        align-items: center;
        justify-content: center;

        @media only screen and (max-width: 992px){
            height: 50vh;

        }

        @media only screen and (max-width: 576px){
            height: 30vh;

        }
    }

    .HomeBanner::before{
        content: '';
        position: absolute;
        top: 100px;
        left: 0;
        width: 100%;
        height: inherit;
        background: rgba(0, 0, 0, 0.5);
        z-index: 0;        
        @media only screen and (max-width: 992px){
            top: 3rem;
        }
    }

    .HomeBannerText{
        color: white;
        font-weight:bold;
        font-size: 6rem;
        z-index: 1;
        @media only screen and (max-width: 992px){
            font-size: 4rem;
        }

        @media only screen and (max-width: 690px){
            word-wrap: break-word;
            text-align: center;
            font-size: 3rem;
        }
        @media only screen and (max-width: 520px){
            font-size: 2.5rem;
        }
    }
</style>