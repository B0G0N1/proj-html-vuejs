<script>
export default {
    props: {
        socialIcons: {
            type: Array,
            required: true
        }
    }
}
</script>

<template>
    <div id="TopHeader">
        <div class="container d-flex justify-content-between py-3">
            <div class="d-flex gap-4">
                <div>
                    <i class="fa-solid fa-envelope me-2" style="color: #c87c34;"></i>
                    <span>info@example.com</span>
                </div>
                <div>
                    <i class="fa-solid fa-phone me-2" style="color: #c87c34;"></i>
                    <span>+1(817)901 3377</span>
                </div>
            </div>
            <div class="d-flex socialIcons gap-1">
                <div v-for="icon in socialIcons" :key="icon.faClass" :style="{backgroundColor: icon.bgColor}">
                    <i :class="icon.faClass"></i>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #TopHeader {
        background-color: #7f7045;

        span {
            color: white;
        }

        .socialIcons {
            i {
                color: white;
            }
            div {
                padding: 1px 5px;
                border-radius: 5px;
            }
        }
    }
</style>