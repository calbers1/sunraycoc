<template>
    <span>
        <div class="main-content pb-4">
            <div class="about-title">
                About Us
            </div>
            <ImageSectionLeft text="Laborum ad exercitation laborum reprehenderit et proident amet mollit ullamco ex incididunt minim. Deserunt tempor sit esse consectetur non ex fugiat eiusmod. Irure aliquip nostrud in nostrud anim est quis id ipsum officia et.">
                <img src="../Assets/tinywow-bible-cross-necklace.jpg" alt="bible with cross necklace"/>
            </ImageSectionLeft>
            <ImageSectionRight text="Duis anim consequat minim pariatur non minim excepteur laboris qui eu ad ullamco. Sunt laborum non ipsum laborum esse fugiat dolor nulla Lorem deserunt ullamco ad. Esse irure minim velit deserunt sunt eiusmod.">
                <img src="../Assets/tinywow-pew-back.jpg" alt="bible with cross necklace"/>
            </ImageSectionRight>
            <ImageSectionLeft text="Laborum ad exercitation laborum reprehenderit et proident amet mollit ullamco ex incididunt minim. Deserunt tempor sit esse consectetur non ex fugiat eiusmod. Irure aliquip nostrud in nostrud anim est quis id ipsum officia et.">
                <img src="../Assets/tinywow-church-building.jpg" alt="bible with cross necklace"/>
            </ImageSectionLeft>
            <ImageSectionRight text="Duis anim consequat minim pariatur non minim excepteur laboris qui eu ad ullamco. Sunt laborum non ipsum laborum esse fugiat dolor nulla Lorem deserunt ullamco ad. Esse irure minim velit deserunt sunt eiusmod.">
                <img src="../Assets/tinywow-bible-stand.jpg" alt="bible with cross necklace"/>
            </ImageSectionRight>
        </div>
    </span>
</template>
	
<script>
import ImageSectionLeft from '~/components/ImageSectionLeft.vue';
import ImageSectionRight from '~/components/ImageSectionRight.vue';
import MainHeader from '~/components/MainHeader.vue';
export default {
    components: { MainHeader, ImageSectionLeft, ImageSectionRight }
}
</script>
	
<style scoped lang="scss">

@import '../Assets/variables.scss';
	.about{
        background-color: $secondary-bg;
    }

    .about-title{
        font-weight:bold;
        font-size: 5rem;
        z-index: 1;
        text-align: center;
        @media only screen and (max-width: 992px){
            font-size: 4rem;
        }

        @media only screen and (max-width: 690px){
            word-wrap: break-word;
            text-align: center;
            font-size: 3rem;
        }
        @media only screen and (max-width: 520px){
            font-size: 2.5rem;
        }
    }
</style>