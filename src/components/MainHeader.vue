<script>
export default {
    props: {
        menuItems: {
            type: Array,
            required: true
        }
    }
}
</script>

<template>
    <div id="MainHeader">
        <div class="container d-flex justify-content-between py-1">
            <img src="../assets/img/logo.png" alt="logo" class="py-2">
            <div class="d-flex align-items-center gap-4">
                <ul class="d-flex gap-4">
                    <li v-for="item in menuItems" :key="item.label">
                        <a :href="item.link">{{ item.label }}</a>
                    </li>                                       
                </ul>
                <button>Get in Toch!</button>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #MainHeader {
        ul {
            list-style-type: none;

            li {
                color: gray;

                &:hover {
                    color: orange;
                }
            }

            a {
                font-size: 1.1rem;
                font-weight: 600;
            }
        }

        button {
            color: white;
            background-color: #cd7c2d;
            font-size: 1.3rem;
            font-weight: 600;
            padding: 12px 20px;
            border-radius: 25px;
            border: none;

            &:hover {
                background-color: #173b65;
            }
        }
    }
</style>