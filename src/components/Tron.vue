<template>
  <v-container>
    <div class="my_container">
      <v-card>
        <v-img class="tron-img"
              src="../assets/images/maxresdefault.jpg"
              aspect-ratio="2.75">
              <div class="title-wrap">
              <h1 class="front-title">FRONTEND DEVELOPER</h1>
              <h2 class="front-subtitle">“Copy-and-Paste was programmed <br>
                  by programmers for programmers.”</h2>
              </div>
        </v-img>
      </v-card>
    </div>
  </v-container>
</template>

<script>
export default {};
</script>

<style lang="scss">

.title-wrap {
  width: 40vw;
  margin-left: 15%;
  margin: 10%;
  
  .front-title {
    color: white;
    border: none;
  }

  .front-subtitle {
    color: white;
  }
}

@media only screen and (max-width: 600px) {
  .front-title {
    color: white;
    font-size: 16px;
    
  }

  .front-subtitle {
    color: white;
    font-size: 16px;
  }
 }

</style>
