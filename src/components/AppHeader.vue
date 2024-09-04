<script>
import TopHeader from './TopHeader.vue';
import MainHeader from './MainHeader.vue';

export default {
    components: {
        TopHeader,
        MainHeader
    },
    data() {
        return {
            socialIcons: [
                { faClass: 'fa-brands fa-square-facebook', bgColor: '#313eb1' },
                { faClass: 'fa-brands fa-pinterest-p', bgColor: 'red' },
                { faClass: 'fa-brands fa-twitter', bgColor: '#81ced0' },
                { faClass: 'fa-brands fa-linkedin-in', bgColor: '#0b61cf' },
                { faClass: 'fa-brands fa-instagram', bgColor: '#ac20ad' }
            ],
            menuItems: [
                { label: "Home", link: "#", isActive: true },
                { label: "About", link: "#", isActive: false },
                { label: "Services", link: "#", isActive: false },
                { label: "Training", link: "#", isActive: false },
                { label: "Blogs", link: "#", isActive: false }
            ]
        }
    }
}
</script>

<template>
    <TopHeader :socialIcons="socialIcons"/>
    <MainHeader :menuItems="menuItems"/>
</template>

<style lang="scss" scoped>

</style>