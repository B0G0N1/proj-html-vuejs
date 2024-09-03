<script>
export default {
    
}
</script>

<template>
    <div id="Newsletter">
        <div class="row h-100">
            <div class="col-6 image-container">
                <img src="../assets/img/news.png" alt="news">
            </div>
            <div class="col-6 d-flex flex-column justify-content-center align-items-start">
                <h2>Subscribe to Our Newsletter</h2>
                <form class="py-2 px-1">
                    <input type="email" placeholder="Your Email Here">
                    <span class="icon ms-2 p-2">@</span>
                </form>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #Newsletter {
        position: absolute;
        top: 0%;
        left: 50%;
        transform: translate(-50%, -50%);
        background-color: #ce7c2a;
        border-radius: 0.7rem;
        width: 800px;
        height: 150px;
        color: white;

        .image-container {
            position: relative;
            
            img {
                position: absolute;
                bottom: 0;
                left: 50%;
                transform: translateX(-50%);
                width: 70%;
            }
        }

        form {
            background-color: white;

            input {
                border: none;
            }

            span {
                background-color: #ce7c2a;
            }
        }
    }
</style>