<script>
import MainFooter from './MainFooter.vue';
import BottomFooter from './BottomFooter.vue';

export default {
    components: {
        MainFooter,
        BottomFooter
    },
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
    }
}
</script>

<template>
    <MainFooter :menuItems="menuItems" :socialIcons="socialIcons"/>
    <BottomFooter/>
</template>

<style lang="scss" scoped>

</style>