<template>
  <section id="TrackSection">
    <div class="track-list container">
        <div class="row">
            <div class="col-3 text-white" v-for="(track,index) in tracks" :key="index">{{track.title}}</div>
        </div>
    </div>
  </section>
</template>

<script>
import axios from "axios";
export default {
  name: "TrackSection",
  data() {
    return {
      tracks: [],
    };
  },
  mounted() {
    axios
      .get("https://flynn.boolean.careers/exercises/api/array/music")
      .then((res) => {
        this.tracks = res.data;
      });
  },
};
</script>


<style scoped>
#TrackSection {
  background-color: #1e2d3b;
  height: 100vh;
}
</style>