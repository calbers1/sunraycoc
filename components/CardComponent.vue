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
        margin: 1rem 0;
        padding: 1rem;
        display: flex;
        height: 90%;
        background-color: $primary-bg;
        align-items: center;
    }

	h4{
        text-align: center;
        @media only screen and (max-width: 992px){
            font-size: 1rem;
        }
    }

    .h-line{
        width: 100%; 
        margin: 0 auto;
        height: 0px;
        border-top: 1px solid black;
        border-radius: 1px;
        padding: 8px 0;
    }

    p, li{
        margin: .5rem .5rem;
    }
    
</style>