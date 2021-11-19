<template>
  <div>
    <Navbar />
    <Slideshow />
    <Slidegroup />
    <Deals />
    <Bagscateg />
    <Bagsec />
  </div>
</template>

<script>
import Slidegroup from "../components/Slidegroup.vue";
import Deals from "../components/Deals.vue";
import Navbar from "../components/Navbar.vue";
import Slideshow from "../components/Slideshow.vue";
import Bagscateg from '../components/Bagscateg.vue';
import Bagsec from '../components/Bagsec.vue'


export default {
  name: "Home",

  components: {
    Navbar,
    Slideshow,
    Slidegroup,
    Deals,
    Bagscateg,
    Bagsec
    
  },
};
</script>
