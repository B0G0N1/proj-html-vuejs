<script>
export default {
    props: {
        title: {
            type: String,
            required: true
        },
        imagePath: {
            type: String,
            required: true
        }
    }
}
</script>

<template>
    <div id="serviceCard">
        <div class="top-semicircle d-flex-center">
            <img :src="imagePath" :alt="title" class="service-image"/>
        </div>
        <div class="square pt-2">
            <h3 class="pb-2">{{ title }}</h3>
            <p>The readable content <br>of a page when <br>looking at its layout.</p>
        </div>
        <div class="bottom-semicircle d-flex-center">
            <div class="circle d-flex-center">
                <img src="../assets/img/right.png" alt="right-arrow">
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #serviceCard {
        width: 200px;

        .square {
            background-color: #ce7c2a;
            color: white;
        }

        .top-semicircle {
            height: 100px;
            background-color: #ce7c2a;
            border-top-left-radius: 100px;
            border-top-right-radius: 100px;

            img {
                width: 80px;
                height: 80px;
            }
        }

        .bottom-semicircle {
            height: 100px;
            background-color: #ce7c2a;
            border-bottom-left-radius: 100px;
            border-bottom-right-radius: 100px;

            .circle {
                background-color: #ffcd01;
                border-radius: 50%;
                padding: 10px;
                
                img {
                    width: 25px;
                    height: 25px;
                }
            }

        }
    }
</style>