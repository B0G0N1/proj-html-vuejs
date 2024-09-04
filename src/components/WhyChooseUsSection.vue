<script>
export default {
    props: {
        whyList: {
            type: Array,
            required: true
        }
    }
}
</script>

<template>
    <div id="WhyChooseUsSection">
            <div class="row">
                <div class="col-6">
                    <img src="../assets/img/why.png" alt="why" class="why">
                </div>
                <div class="col-6 p-3">
                    <div class="d-flex align-items-center gap-3">
                        <img src="../assets/img/dog-icon.png" alt="dog-icon">
                        <span>About Us</span>
                    </div>
                    <p class="my-3">Why Choose Us ?</p>
                    <div v-for="reason in whyList" :key="reason.title" class="row">
                        <div :class="'col-' + reason.spaceCol"></div>
                        <div class="col-2 d-flex">
                            <img :src="reason.image" alt="w-3" class="icon">
                        </div>
                        <div :class="'col-' + reason.textCol + ' p-3'">
                            <p class="mb-2"><strong>{{ reason.title }}</strong></p>
                            <p>It is a long established fact that a reader will be distructed by the readable content of a
                                page when looking at its layout.</p>
                        </div>
                    </div>
                </div>
            </div>
    </div>
</template>

<style lang="scss" scoped>
    #WhyChooseUsSection {
        .why {
            width: 100%;
        }

        .icon {
            width: 100%;
        }
    }
</style>