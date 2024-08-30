<script>
export default {
    
}
</script>

<template>
    <div id="AboutSection">
        <div class="container">
            <div class="row">
                <div class="col-6 p-5">
                    <img src="../assets/img/about.png" alt="about" class="dog">
                </div>
                <div class="col-6 py-5 d-flex flex-column justify-content-center">
                    <div class="d-flex align-items-center gap-3">
                        <img src="/dog-icon.png" alt="">
                        <span>About Us</span>
                    </div>
                    <h4 class="my-3">Welcome DogMilo Pets</h4>
                    <p>Lorem Ipsum is simply dummy text of the printing and typesetting
                        industry. Lorem Ipsum has been the industry's standard dummy text
                        ever since the 1500s, when an unknown printer took a galley of type
                        and scrambled</p>
                    <p class="mt-3">Lorem Ipsum is simply dummy text of the printing and typesetting
                        industry. Lorem Ipsum has been the industry's standard dummy text
                        ever since the 1500s, when an unknown printer took a galley of type
                        and scrambled</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #AboutSection {
        .dog {
            width: 100%;
        }

        h4 {
            font-size: 2.3rem;
        }
    }
</style>