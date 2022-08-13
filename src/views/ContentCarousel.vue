<template>
    <div class="view-carousel">
        <Carousel
            @next="next"
            @prev="prev"
        >
            <!-- <img src="https://picsum.photos/id/237/600/350" alt=""> -->
            <CarouselSlide 
            v-for="(slide,index) in slides" 
            :index="index" 
            :visibleSlide="visibleSlide"
            v-bind:key="slide.id">
                <!-- <img src="slide"> -->
                <h1>{{ slide }}</h1>
            </CarouselSlide>
        </Carousel>
    </div>
</template>

<script>
import Carousel from '@/components/Em-Carousel.vue';
import CarouselSlide from '@/components/CarouselSlide.vue';

export default {
    data() {
        return {
            slides: [
                // 'https://picsum.photos/id/237/600/350',
                // 'https://picsum.photos/id/238/600/350',
                // 'https://picsum.photos/id/239/600/350',
                // 'https://picsum.photos/id/240/600/350',
                // 'https://picsum.photos/id/241/600/350',
                // 'https://picsum.photos/id/242/600/350',
                'apple',
                'banana',
                'fine',
                'ork',
            ],
            visibleSlide: 0,
        }
    },
    // If 'methods' code gets complicated, use 'computed' better. 
    computed: {
        slidesLen () {
            return this.slides.length;
        }
    },
    methods: {
        next() {
            if(this.visibleSlide >= this.slidesLen - 1) {
                this.visibleSlide = 0;
            }
            else {
                this.visibleSlide++;
            }
        },
        prev() {
            if(this.visibleSlide <= 0 ) {
                this.visibleSlide = this.slidesLen -1;
            }
            else {
                this.visibleSlide--;
            }
        },
    },
    components: {
        Carousel,
        CarouselSlide,
    }
}
</script>

<style scoped>
.view-carousel {
    display: flex;
    justify-content: center;
}
</style>