<template>
    <span>
        <HomeBanner />
        <div class="row blurble">
            <div class="col-12 col-lg-8 offset-lg-2 col-xl-6 offset-xl-3 blurb">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Distinctio nostrum aliquam ab debitis quia magnam ea temporibus. (Mission statement/scripture/small blurb)
            </div>
        </div>
        <div class="main-content">
            <div class="row pt-4">

                <div class="col-12 col-xl-6">
                    <CardComponent title="Service Schedule">
                        <div class="col-12">
                            <p>Sunday: 9AM and 6PM</p>
                        </div>
                        <div class="col-12">
                            <p>Wednesday: 7PM</p>
                        </div>
                    </CardComponent>
                </div>
                <div class="col-12 col-xl-6">
                    <CardComponent title="Location">
                        <p>7th & Ave. N Sunray, Texas</p>
                    </CardComponent>
                </div>
            </div>
        </div>
    </span>
</template>
	
<script setup>
import HomeBanner from '~/components/HomeBanner.vue';

</script>
	
<style scoped lang="scss">

    @import '../assets/variables.scss';


    .blurble{
        background-color: $primary-bg;
    }
    .blurb{
        font-size: large;
        font-style: italic;
        color: $primary;
        padding: 2rem;
        word-wrap: break-word;
    }
    .mission{
        font-size: 3rem;
    }
    
    .main-content{
        background-color: $secondary-bg;
        color: $primary;
        padding: 0 1rem;
        height: calc(100vh - 100px);
        @media only screen and (max-width: 992px){
            height: calc(100vh - 3rem);
        }
    }
	
</style>