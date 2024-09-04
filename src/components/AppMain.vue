<script>
import HeroSection from './HeroSection.vue';
import AboutSection from './AboutSection.vue';
import ServicesSection from './ServicesSection.vue';
import WhyChooseUsSection from './WhyChooseUsSection.vue';
import TestimonialsSection from './TestimonialsSection.vue';

export default {
    components: {
        HeroSection,
        AboutSection,
        ServicesSection,
        WhyChooseUsSection,
        TestimonialsSection
    },
    data() {
        return {
            servicesList: [
                { title: 'Pet Sitting', imagePath: '/src/assets/img/d-1.png' },
                { title: 'Puppy Sitting', imagePath: '/src/assets/img/d-2.png' },
                { title: 'Dog Walking', imagePath: '/src/assets/img/d-3.png' },
                { title: 'Night Care', imagePath: '/src/assets/img/d-4.png' },
                { title: 'Pet Sitting', imagePath: '/src/assets/img/d-5.png' }
            ],
            whyList: [
                { title: "Safety First", image: "/src/assets/img/w-3.png", spaceCol: "0", textCol: "10" },
                { title: "Play Yards", image: "/src/assets/img/w-2.png", spaceCol: "2", textCol: "8" },
                { title: "Monitor Your Pets", image: "/src/assets/img/w-1.png", spaceCol: "4", textCol: "6" }
            ],
            testimonialsList: [
                {
                    rating: 5,
                    name: "Tobias May",
                    profession: "UI/UX Designer",
                    review: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when...",
                    title: "Great Place",
                    image: "/src/assets/img/t1.png"
                },
                {
                    rating: 5,
                    name: "Tobias May",
                    profession: "UI/UX Designer",
                    review: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when...",
                    title: "Great Place",
                    image: "/src/assets/img/t1.png" 
                }
            ]
        }
    }
}
</script>

<template>
    <HeroSection/>
    <AboutSection/>
    <ServicesSection :servicesList="servicesList"/>
    <WhyChooseUsSection :whyList="whyList"/>
    <TestimonialsSection :testimonialsList="testimonialsList"/>
</template>

<style lang="scss" scoped>

</style>