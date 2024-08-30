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
        <div class="top-semicircle d-flex justify-content-center align-items-center">
            <img :src="imagePath" :alt="title" class="service-image" />
        </div>
        <div class="square">
            <h3>{{ title }}</h3>
            <p>The readable content <br>of a page when <br>looking at its layout.</p>
        </div>
        <div class="bottom-semicircle d-flex justify-content-center align-items-center">
            <div class="circle d-flex justify-content-center align-items-center">
                <img src="../assets/img/right.png" alt="right-arrow">
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #serviceCard {
        width: 200px;

        .square {
            background-color: orange;
            color: white;
        }

        .top-semicircle {
            height: 150px;
            background-color: orange;
            border-top-left-radius: 100%;
            border-top-right-radius: 100%;

            img {
                width: 100px;
                height: 100px;
            }
        }

        .bottom-semicircle {
            height: 150px;
            background-color: orange;
            border-bottom-left-radius: 100%;
            border-bottom-right-radius: 100%;

            .circle {
                background-color: #fecc02;
                border-radius: 50%;
                padding: 20px;
                
                img {
                    width: 30px;
                    height: 30px;
                }
            }

        }
    }

    * {
        border: 1px dashed red;
    }
</style>