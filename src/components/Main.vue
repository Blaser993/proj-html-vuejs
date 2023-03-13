<template>

    <MainFeature></MainFeature>
    <MainCompany></MainCompany>
    <MainServices></MainServices>
    <MainPricing></MainPricing>
    <MainNews></MainNews>
    <MainNewsletter></MainNewsletter>
    <MainContacts></MainContacts>

</template>

<script>
import MainFeature from "./MainFeature.vue";
import MainCompany from "./MainCompany.vue";
import MainServices from "./MainServices.vue";
import MainPricing from "./MainPricing.vue";
import MainNews from "./MainNews.vue";
import MainNewsletter from "./MainNewsletter.vue";
import MainContacts from "./MainContacts.vue";

export default {
    components:{
        MainFeature,
        MainCompany,
        MainServices,
        MainPricing,
        MainNews,
        MainNewsletter,
        MainContacts
    }
}
</script>

<style lang="scss" scoped> 

</style>