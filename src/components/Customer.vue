<template>
    <section id="carousel" class="bg-primary py-5">
        <div class="container">
            <app-title title-value="customers" subtitle-value="Lorem ipsum dolor sit amet." color="light"></app-title>
            <div class="row mt-5">
                <div class="col-md-8 mx-auto text-center">
                    <app-carousel :items="items"></app-carousel>
                </div>
            </div>
        </div>
    </section>
</template>
<script>

import imgProject1 from '../assets/projects/project1.jpg'
import imgProject2 from '../assets/projects/project2.jpg'
import imgProject3 from '../assets/projects/project3.jpg'
import Carousel from './common/Carousel.vue'

export default {
    data () {
        return {
            items: [{image: imgProject1, active: true}, {image: imgProject2, active: false}, {image: imgProject3, active: false}]
        }
    },
    components: {
        appCarousel: Carousel
    }
}
</script>
