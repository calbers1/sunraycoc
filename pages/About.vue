<template>
    <span>
        <div class="main-content pt-5 pb-5">
            <ImageSectionLeft text="Laborum ad exercitation laborum reprehenderit et proident amet mollit ullamco ex incididunt minim. Deserunt tempor sit esse consectetur non ex fugiat eiusmod. Irure aliquip nostrud in nostrud anim est quis id ipsum officia et. Duis anim consequat minim pariatur non minim excepteur laboris qui eu ad ullamco. Sunt laborum non ipsum laborum esse fugiat dolor nulla Lorem deserunt ullamco ad. Esse irure minim velit deserunt sunt eiusmod.">
                <img src="../Assets/tinywow-bible-cross-necklace.jpg" alt="bible with cross necklace"/>
            </ImageSectionLeft>
        </div>
    </span>
</template>
	
<script>
import ImageSectionLeft from '~/components/ImageSectionLeft.vue';
import MainHeader from '~/components/MainHeader.vue';
export default {
    components: { MainHeader, ImageSectionLeft }
}
</script>
	
<style scoped lang="scss">

@import '../Assets/variables.scss';
	.about{
        background-color: $secondary-bg;
    }
</style>