<script>
import TestimonialCard from './TestimonialCard.vue';

export default {
    components: {
        TestimonialCard
    },
    data() {
        return {
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
    <div id="TestimonialsSection">
        <div class="container d-flex justify-content-evenly py-5">
            <div class="about-us">
                <div class="d-flex align-items-center gap-2">
                    <img src="../assets/img/dog-icon.png" alt="">
                    <span>About Us</span>
                </div>
                <p class="fs-5 fw-medium my-3">Over 8000 Customers <br>With 5-Star Review</p>
                <p class="review mb-3">It is a long established fact that a reader will be distructed by the readable content of a page when looking at its layout.</p>
                <span class="star" v-for="n in 5" :key="'star' + n">&#9733;</span>
            </div>
            <TestimonialCard v-for="testimonial in testimonialsList" :key="testimonial.name" :testimonial="testimonial"/>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #TestimonialsSection {
        display: flex;
        justify-content: center;
        padding-bottom: 9rem;

        .about-us {
            height: 300px;
            width: 300px;
            padding: 20px;
            border-radius: 5px;

            img {
                height: 25px;
                width: 25px;
            }
        }

        .star {
            color: #f5c518;
        }

        .review {
            font-size: 1em;
            color: #666;
        }
    }
</style>