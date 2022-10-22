<template>
  <div class="home-page">

    <HomeImage/>
    <CheckupBar class="checkup-bar"/>
    <MajorResources/>
    <HPWelcomeTo></HPWelcomeTo>
    <HPContactUs/>
    <HPServices/>
    <HPReviews/>
  </div>

</template>

<style scoped>
.home-page{
  display: flex;
  flex-direction: column;
}
.checkup-bar{
  z-index: 101;
}

</style>

<script>
import HomeImage from "../components/HomeImage.vue";
import CheckupBar from "@/components/Checkup-Bar.vue";
import MajorResources from "../components/Major-Resources.vue";
import HPWelcomeTo from "@/components/HP-welcome-to.vue";
import HPContactUs from "../components/ContactUs.vue";
import HPServices from "../components/HP-Services.vue";
import HPReviews from "../components/HP-Reviews.vue";
// @ is an alias to /src



export default {
  name: 'HomeView',
  components: {
    HomeImage,
    CheckupBar,
    MajorResources,
    HPWelcomeTo,
    HPContactUs,
    HPServices,
    HPReviews
}
}
</script>
