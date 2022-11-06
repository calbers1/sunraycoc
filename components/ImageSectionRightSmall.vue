<template>
    <span>
        <div class="row ImageSectionRightSmall pl-0 pl-lg-3">
            <div class="col-12 col-lg-6 text-col">
                <p class="text">{{text}}</p>
            </div>
            <div class="col-12 col-lg-6 img-col">
                
            <div class="title col-12 text-center">{{title}}</div>
                <slot></slot>
            </div>
        </div>
    </span>
</template>
	
<script setup>
    const props = defineProps({
        text: String,
        title: String,
    })
</script>
	
<style lang="scss" scoped>

@import '../Assets/variables.scss';

.title{
    font-size: 1.5rem;
}

.ImageSectionRightSmall{
    margin: 0 1rem 1rem 1rem;
    background: $primary-bg;
    border-radius: 5px;
    flex-wrap: wrap-reverse;
}

.img-col{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    padding-bottom: 1.5rem;
}

img{
    width: 100%;
    border-radius: 5px;
    height: auto;
    max-height: 80%;

    max-width: 400px;
    object-fit: cover;
    object-position: center center;
    @media only screen and (max-width: 990px) {
        width: 70%;
    }
    @media only screen and (max-width: 600px) {
        width: 100%;
    }
}

.text-col{
    display: flex;
}
.text{
    font-size: 1.75rem;
    justify-self: center;
    align-self: center;
    color: $primary;
    @media only screen and (max-width: 600px) {
        font-size: 1.25rem;
    }
}
	
</style>