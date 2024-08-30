<script>
import ServiceCard from './ServiceCard.vue';

export default {
    components: {
        ServiceCard
    },
    data() {
        return {
            servicesList: [
                { title: 'Pet Sitting', imagePath: '/d-1.png' },
                { title: 'Puppy Sitting', imagePath: '/d-2.png' },
                { title: 'Dog Walking', imagePath: '/d-3.png' },
                { title: 'Night Care', imagePath: '/d-4.png' },
                { title: 'Pet Sitting', imagePath: '/d-5.png' }
            ]
        }
    }
}
</script>

<template>
    <div id="ServiceSection">
        <div class="container text-center py-3">
            <p>Service</p>
            <p class="my-3 title">Dog Milo Pet Care Services <br>For Your Best Friend</p>
            <div class="d-flex justify-content-between">
                <ServiceCard v-for="service in servicesList" :key="service.title" :title="service.title" :image-path="service.imagePath"/>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #ServiceSection {
        background-color: #f5f5f5;

        .title {
            font-size: 2rem;
        }
    }
</style>