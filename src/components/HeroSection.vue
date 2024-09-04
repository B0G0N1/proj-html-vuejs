<script>
export default {
    
}
</script>

<template>
    <div id="HeroSection">
        <div class="container py-5">
            <p><strong>Welcome to</strong><br> DogMilo <strong>Pets</strong></p>
            <p class="my-2">Lorem Ipsum is simply dummy text of the printing <br>and typesetting industry.</p>
            <div class="d-flex align-items-center gap-2 mt-3">
                <button>Get Started</button>
                <img src="../assets/img/play.png" alt="play">
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #HeroSection {
        background-image: url(../assets/img/b.png);
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        color: white;
        padding: 4rem 0;

        h4 {
            font-size: 2rem;
        }

        p:first-child {
            font-size: 2rem;
        }

        button {
            color: white;
            background-color: #cd7c2d;
            font-size: 1.3rem;
            font-weight: 600;
            padding: 12px 20px;
            border-radius: 25px;
            border: none;
        }

        img {
            background-color: #70d1f3;
            height: 45px;
            padding: 10px;
            border-radius: 10%;
        }
    }
</style>