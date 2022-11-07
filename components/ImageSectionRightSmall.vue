<template>
    <span>
        <div class="row ImageSectionRightSmall pl-0 pl-lg-3" :class="{_shadow: shadow}">
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
        shadow: Boolean,
    })
</script>
	
<style lang="scss" scoped>
@import '../Assets/variables.scss';

.title{
    font-size: 1.5rem;
}

.ImageSectionRightSmall{
    border: 2px solid $primary;
    margin: 0 1rem 1rem 1rem;
    background: $primary-bg;
    border-radius: 5px;
    flex-wrap: wrap-reverse;
}

._shadow {
    border: none !important;
    box-shadow: 0px 0px 10px 0px rgba(144, 154, 161, 0.75);
    -webkit-box-shadow: 0px 0px 10px 0px rgba(144, 154, 161, 0.75);
    -moz-box-shadow: 0px 0px 10px 0px rgba(144, 154, 161, 0.75);
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

.text-col {
    display: flex;
    justify-content: end;
    align-items: center;
    @media only screen and (max-width: 992px) {
        justify-content: center;
    }
}
.text{
    font-size: 1.75rem;
    color: $primary;
    width: 80%;
    @media only screen and (max-width: 600px) {
        font-size: 1.25rem;
        width: 100%;
    }
}
</style>