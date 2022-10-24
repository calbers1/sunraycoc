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
    console.log(props);

</script>
	
<style lang="scss" scoped>

    .card{
        border: 1px solid black;
        margin: 1rem 0;
        padding: 1rem;
        display: flex;
        height: 90%;
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

    p{
        text-align: center;
        margin: auto 0
    }
</style>