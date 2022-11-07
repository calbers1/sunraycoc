<template>
    <span>
        <div class="HomeBanner">
            <div class="HomeBannerTextContainer">
                <div class="HomeBannerText">
                    <span class="front">Welcome</span> <span class="back">to Sunray!</span>
                </div>
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
        background-attachment: fixed;
        height: 75vh;
        display: flex;
        align-items: center;
        justify-content: center;

        @media only screen and (max-width: 992px){
            height: 50vh;
            background-position: 50% -15rem;
        }

        @media only screen and (max-width: 576px){
            height: 30vh;
            background-size: contain;
            background-position: 0% 7%;
        }

        @media only screen and (max-width: 430px){
            height: 30vh;
            background-position: top;
            background-image: url('~/Assets/tinywow-church-building.jpg');
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
        transform: translateY(-10rem);
        animation-name: slide-up;
        animation-duration: 2s;
        animation-delay: 1s;
        animation-fill-mode: forwards;
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

    .HomeBannerTextContainer{
        overflow: hidden;
        z-index: 1;
    }


    //animation stuff
    @keyframes slide-up{
        0%{
            transform: translateY(-10rem);
        }
        100%{
            transform: translateY(0px);
        }
    }
</style>