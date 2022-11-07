<template>
    <span>
        <div class="card">
            <h4>{{title}}</h4>
            <div class="h-line"></div>
            <p><slot/></p>
        </div>
    </span>
</template>
	
<script setup>

    const props = defineProps({
        title: String,
    })

</script>
	
<style lang="scss" scoped>

@import '../Assets/variables.scss';
    .card{
        border: none;
        border-radius: 0;
        margin: 1rem 0 0 0;
        padding: 1rem;
        padding-bottom: 2.5rem;
        display: flex;
        height: 90%;
        background-color: $primary-bg;
        align-items: center;

        @media only screen and (max-width: 600px){
            height: 93%;

        }

        @media only screen and (max-width: 570px){
            height: 90%;
        }

        @media only screen and (max-width: 436px){
            height: 93%;
        }
    }

	h4{
        text-align: center;
        @media only screen and (max-width: 992px){
            font-size: 1rem;
        }
    }

    p, li{
        margin: .5rem .5rem;
    }
    
</style>