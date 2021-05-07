<template>
  <v-content>
    <Tron />
    <Skills />
    <Gallery />
    
    <div class="video-wrap">
      <iframe class="video" height="315" src="https://www.youtube.com/embed/3G6N2txvG6A" title="YouTube video player" frameborder="0" allow="" allowfullscreen></iframe>
    </div>
  </v-content>
</template>

<script>
import Tron from "../components/Tron";
import Gallery from "../components/Gallery";
import Skills from "../components/Skills";

export default {
  name: "Home",

  components: {
    Gallery,
    Skills,
    Tron
    
  }
};
</script>