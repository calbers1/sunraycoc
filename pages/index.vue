<template>
    <span>
        <HomeBanner />
        <div class="row blurble">
            <div class="col-12 col-lg-8 offset-lg-2 col-xl-6 offset-xl-3 blurb">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Distinctio nostrum aliquam ab debitis quia magnam ea temporibus. (Mission statement/scripture/small blurb)
            </div>
        </div>
        <div class="main">
            <div class="row pt-4">

                <div class="col-12 col-xl-6">
                    <CardComponent title="Service Schedule">
                        <div class="col-12">
                            <p>Sunday: 9:00 AM and 6:00 PM</p>
                        </div>
                        <div class="col-12">
                            <p>Wednesday: 7:00 PM</p>
                        </div>
                    </CardComponent>
                </div>
                <div class="col-12 col-xl-6">
                    <CardComponent title="Location">
                        <p><a href="http://maps.apple.com/?daddr=700+S+Ave+N,+Sunray+TX">7th & Ave N, Sunray, Texas 79086</a></p>
                    </CardComponent>
                </div>

                <div class="col-12">
                    <CardComponent title="Classes">
                        <ul>
                            <li>Adults: Mollit do elit Lorem exercitation pariatur nostrud laboris magna cupidatat anim consequat ipsum est.</li>
                            <li>Teens: Aliqua laboris voluptate eiusmod reprehenderit irure excepteur do mollit duis duis.</li>
                            <li>Elementary: Anim in occaecat nostrud pariatur duis tempor ipsum Lorem do aliquip.</li>
                            <li>Kindergarden: Aliqua exercitation tempor in officia commodo in qui.</li>
                            <li>Pre-K: Eiusmod tempor pariatur ullamco et excepteur aliqua esse occaecat cillum laboris enim laborum non ad.</li>
                            <li>Nursery: Incididunt officia minim nisi fugiat eu dolor.</li>
                        </ul>

                    </CardComponent>
                </div>

                <div class="col-12 col-xl-6 t-minus-1">
                    <MediaBanner title="Placeholder" text="Et incididunt tempor incididunt proident tempor deserunt mollit culpa sint." link="/" link-text="Link">
                        <img src="../Assets/img8.jpg" />
                    </MediaBanner>
                </div>
                <div class="col-12 col-xl-6 mt-1 mt-xl-0">
                    <MediaBanner title="Placeholder" text="Et incididunt tempor incididunt proident tempor deserunt mollit culpa sint." link="/" link-text="Link">
                        <img src="../Assets/img12.jpg" />
                    </MediaBanner>
                </div>

            </div>
        </div>
    </span>
</template>
	
<script setup>
import CardComponent from '~/components/CardComponent.vue';
import HomeBanner from '~/components/HomeBanner.vue';
import MediaBanner from '~/components/MediaBanner.vue';

if ( process.server )
{
    console.log( "THIS IS ON THE SERVER." );
}

</script>
	
<style scoped lang="scss">
@import '../Assets/variables.scss';

.t-minus-1 {
    @media only screen and (max-width: 570px) {

        margin-top: -1rem;
    }
}

.blurble {
    background-color: $secondary-bg;
    margin: 0;
}

.blurb {
    font-size: large;
    font-style: italic;
    color: $primary;
    padding: 2rem;
    word-wrap: break-word;
}

.mission {
    font-size: 3rem;
}

p>a {
    color: adjust-color($color: $primary, $lightness: 20%)
}

p>a:hover {
    color: $primary;
}

.card {
    box-shadow: 0px 5px 9px 1px rgba(0, 0, 0, 0.43);
    -webkit-box-shadow: 0px 5px 9px 1px rgba(0, 0, 0, 0.43);
    -moz-box-shadow: 0px 5px 9px 1px rgba(0, 0, 0, 0.43);
}
</style>