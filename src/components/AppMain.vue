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
    }
}
</script>

<template>
    <HeroSection/>
    <AboutSection/>
    <ServicesSection/>
    <WhyChooseUsSection/>
    <TestimonialsSection class="mb-5"/>
</template>

<style lang="scss" scoped>

</style>