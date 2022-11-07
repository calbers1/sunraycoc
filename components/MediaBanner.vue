<template>
    <span>
        <div class="card">
        <slot class="card-img-top"></slot>
        <div class="card-body">
            <h5 class="card-title">{{title}}</h5>
            <div class="h-line"></div>
            <p class="card-text">{{text}}</p>
            <a :href="link" class="btn btn-primary">{{linkText}}</a>
        </div>
    </div>
    </span>
</template>
	
<script setup>
    const props = defineProps({
        title: String,
        text: String,
        link: String,
        linkText: String,
    })

</script>
	
<style lang="scss" scoped>

@import '../Assets/variables.scss';
    .card{
        border: none;
        border-radius: 0;
        padding: 1rem 0 2rem 0;
        display: flex;
        height: 97%;
        background-color: $primary-bg;
    }

    img{
        position: relative;
        max-width: 90%;
        max-height: 300px;
        margin: 0 auto;
        object-fit: contain;
        object-position: center center;
    }

	h5{
        text-align: center;
        @media only screen and (max-width: 992px){
            font-size: 1rem;
        }
    }


    p{
        text-align: center;
        margin: auto 0
    }

    .btn{
        margin-top: 2rem;
        margin-bottom: -1rem;
        width: 100%;
        background: $primary;
    }

    .btn:hover{
        background: adjust-color($color: $primary, $lightness: 10%)
    }
</style>