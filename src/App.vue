<template>
  <div>
    <TheHeader></TheHeader>
    <TrackSection></TrackSection>
  </div>
</template>

<script> 

import TheHeader from "./components/TheHeader.vue";
import TrackSection from "./components/TrackSection.vue";
export default {
  name: "App",
  components: {
    TheHeader : TheHeader,
    TrackSection : TrackSection,
    
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
