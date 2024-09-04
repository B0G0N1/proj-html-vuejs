<script>
import ServiceCard from './ServiceCard.vue';

export default {
    components: {
        ServiceCard
    },
    props: {
        servicesList: {
            type: Array,
            required: true
        }
    }
}
</script>

<template>
    <div id="ServiceSection">
        <div class="container text-center py-5">
            <h3 class="fw-medium">Service</h3>
            <h3 class="mt-4 mb-5 fs-4 fw-medium">Dog Milo Pet Care Services <br>For Your Best Friend</h3>
            <div class="d-flex justify-content-between">
                <ServiceCard v-for="service in servicesList" :key="service.title" :title="service.title" :image-path="service.imagePath"/>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #ServiceSection {
        background-color: #f5f5f5;
        background-image: 
            url('../assets/img/dog-left.png'),
            url('../assets/img/dog-logo.png');
        background-position: top 20px left 0, top 20px right 0;
        background-size: 15% auto, 15% auto;
        background-repeat: no-repeat;

        p {
            color: gray;
        }
    }
</style>