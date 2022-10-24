<template>
    <span>
        <MainHeader></MainHeader>
        <div class="main-content">
            <div class="row">
                <div class="col-12 text-center mt-5">
                    <div class="home-title">Welcome!</div>
                </div>

                <div class="col-12 col-xl-4">
                    <CardComponent title="Service Schedule">
                        <div class="col-12">
                            <p>Sunday: 9AM and 6PM</p>
                        </div>
                        <div class="col-12">
                            <p>Wednesday: 7PM</p>
                        </div>
                    </CardComponent>
                </div>
                <div class="col-12 col-xl-4">
                    <CardComponent title="Location">7th & Ave. N Sunray, Texas</CardComponent>
                </div>
                <div class="col-12 col-xl-4">
                    <CardComponent title="Email">sunraycofc@gmail.com</CardComponent>
                </div>
            </div>
        </div>
    </span>
</template>
	
<script>
import MainHeader from '~/components/MainHeader.vue';
import CardComponent from '~/components/CardComponent.vue';
export default {
    components: { MainHeader, CardComponent }
}
</script>
	
<style scoped lang="scss">

    @import '../assets/variables.scss';

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

    .home-title{
        @media only screen and (max-width: 992px){
            font-size: 4rem;
        }

        @media only screen and (max-width: 576px){
            font-size: 2rem;
        }

        font-weight: bold;
        font-size: 6rem;
    }
	
</style>