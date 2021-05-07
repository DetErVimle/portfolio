<template>
  <div class="block galleryBlock">
    <v-container>
      <h2 class="my-title text-center">PORTFOLIO</h2>
      <v-row>
        <v-col v-for="item in items" :key="item.id" class="d-flex child-flex" cols="6" sm="4">
          <v-card flat tile class="d-flex">
            <v-img :src="item.src" max-height="180" max-width="100%" class="grey lighten-2">
              <template v-slot:placeholder>
                <v-row class="fill-height ma-0" align="center" justify="center">
                  <v-progress-circular indeterminate color="grey lighten-5"></v-progress-circular>
                </v-row>
              </template>
            </v-img>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "Gallery",
  data() {
    return {
      items: [
        {
          id: 1,
          src: require("../assets/images/coralrelief.jpg")
        },
        {
          id: 2,
          src: require("../assets/images/PC_Landscape_Peter.jpg")
        },
        {
          id: 3,
          src: require("../assets/images/img3.jpg")
        },
        {
          id: 4,
          src: require("../assets/images/img4.jpg")
        },
        {
          id: 5,
          src: require("../assets/images/img5.jpg")
        },
        {
          id: 6,
          src: require("../assets/images/img6.jpg")
        },
        
      ]
    };
  }
};
</script>