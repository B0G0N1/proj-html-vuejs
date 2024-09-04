<script>
import Newsletter from './Newsletter.vue'

export default {
    data() {
        return {
            menuItems: [
                {
                    title: "Support",
                    elements: ["Contact Us", "Online Chat", "Whatsapp", "Telegram", "Snapchat"]
                },
                {
                    title: "About",
                    elements: ["About Us", "Blog", "Career", "Job", "In press"]
                },
                {
                    title: "Faq",
                    elements: ["Account", "Order", "Delivery", "Payment", "Return"]
                }
            ],
            socialIcons: [
                { faClass: 'fa-brands fa-square-facebook', bgColor: '#313eb1' },
                { faClass: 'fa-brands fa-pinterest-p', bgColor: 'red' },
                { faClass: 'fa-brands fa-twitter', bgColor: '#81ced0' },
                { faClass: 'fa-brands fa-linkedin-in', bgColor: '#0b61cf' },
                { faClass: 'fa-brands fa-instagram', bgColor: '#ac20ad' }
            ]
        }
    },
    components: {
        Newsletter
    }
}
</script>

<template>
    <div id="MainFooter">
        <Newsletter/>
        <div class="container d-flex justify-content-between py-5">
            <div>
                <h3>Get in Touch</h3>
                <p class="my-4">Have a Question for us? <br>we'll answer your problem here</p>
                <div class="d-flex socialIcons gap-1">
                    <div v-for="icon in socialIcons" :key="icon.faClass" :style="{backgroundColor: icon.bgColor}">
                        <i :class="icon.faClass"></i>
                    </div>
                </div>
            </div>
            <div v-for="menu in menuItems" :key="menu.title" class="justify-content-evenly">
                <h3>{{ menu.title }}</h3>
                <ul class="list-unstyled">
                    <li v-for="item in menu.elements" :key="item">{{ item }}</li>
                </ul>
            </div>
            <div>
                <h3>Contact me</h3>
                <div>
                    <i class="fa-solid fa-location-arrow me-2" style="color: #c87c34;"></i>
                    <span>4500 Mercantile plaza,suite <br>300, fort worth, TX, 76137, USA</span>
                </div>
                <div>
                    <i class="fa-solid fa-envelope me-2 my-3" style="color: #c87c34;"></i>
                    <span>info@example.com</span>
                </div>
                <div>
                    <i class="fa-solid fa-phone me-2" style="color: #c87c34;"></i>
                    <span>+1(817)901 3377</span>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    #MainFooter {
        position: relative;
        background-color: black;
        padding-top: 5rem;

        h3 {
            color: orange;
            margin-bottom: 1rem;
        }

        p, span, li {
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