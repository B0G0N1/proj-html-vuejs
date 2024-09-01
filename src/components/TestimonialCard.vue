<script>
export default {
    props: {
        testimonial: {
            type: Object,
            required: true
        }
    }
}
</script>

<template>
    <div id="TestimonialCard">
        <div class="mb-2">
            <span v-for="star in 5" :key="star" class="star" :class="{'filled': star <= testimonial.rating}">&#9733;</span>
        </div>
        <h3>{{ testimonial.title }}</h3>
        <p class="review mb-4">{{ testimonial.review }}</p>
        <div class="d-flex gap-1">
            <img :src="testimonial.image" alt="Profile picture" class="profile-img"/>
            <div>
                <p class="fw-bold">{{ testimonial.name }}</p>
                <p class="profession">{{ testimonial.profession }}</p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #TestimonialCard {
        background-color: #f4f4f4;
        height: 300px;
        width: 300px;
        padding: 20px;
        border-radius: 5px;
        
        .star {
            color: #ddd;
        }
        
        .star.filled {
            color: #f5c518;
        }
        
        .review {
            font-size: 1em;
            color: #666;
        }
        
        .profile-img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-right: 10px;
        }
        
        .profession {
            font-size: 0.9em;
            color: #888;
        }
    }
</style>