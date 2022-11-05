<template>
    <span>
        <div class="row ImageSectionLeft">
            <div class="col-12 col-lg-6 img-col">
                <slot></slot>
            </div>
            <div class="col-12 col-lg-6 text-col">
                <p class="text">{{text}}</p>
            </div>
        </div>
    </span>
</template>
	
<script setup>
    const props = defineProps({
        text: String,
    })
</script>
	
<style lang="scss" scoped>

@import '../Assets/variables.scss';

.ImageSectionLeft{
    padding: 1rem;
    margin: 1rem;
    background: $primary-bg;
    border-radius: 5px;
}

.img-col{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
}

img{
    width: 80%;
    border-radius: 5px;
    height: auto;

    max-width: 700px;
    object-fit: cover;
    object-position: center center;
    @media only screen and (max-width: 990px) {
        width: 70%;
        margin-bottom: 2rem;
    }
    @media only screen and (max-width: 600px) {
        width: 90%;
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
}
	
</style>