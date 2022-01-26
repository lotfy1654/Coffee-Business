<template>
  <div id="app">
    <app-header />
    <dark-coffe />
    <cold-coffee />
    <hot-coffee />
    <!-- <gift-coffee /> -->
    <!-- <about-us /> -->
    <!-- <customer-reviews /> -->
    <!-- <our-pranches /> -->
    <!-- <end-footer /> -->
    <router-view />
  </div>
</template>

<script>
import AppHeader from "@/components/global/AppHeader.vue";
import DarkCoffe from "@/components/global/DarkCoffe.vue";
import ColdCoffee from "@/components/global/ColdCoffee.vue";
import HotCoffee from "@/components/global/HotCoffee.vue";
// import GiftCoffee from "@/components/global/GiftCoffee.vue";
// import AboutUs from "@/components/global/AboutUs.vue";
// import CustomerReviews from "@/components/global/CustomerReviews.vue";
// import OurPranches from "@/components/global/OurPranches.vue";
// import EndFooter from "@/components/global/EndFooter.vue";

export default {
  components: {
    AppHeader,
    DarkCoffe,
    ColdCoffee,
    HotCoffee,
    // GiftCoffee,
    // AboutUs,
    // CustomerReviews,
    // OurPranches,
    // EndFooter,
  },
};
</script>

<style lang="scss">
@import "../src/assets/style/_variables.scss";
</style>
