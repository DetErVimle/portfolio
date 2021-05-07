<template>
<v-container>
    <h2 style="color: white;font-size:30px;" class="my-title text-center">SKILLS</h2>
    <div class="box-wrap">
        <div class="box">
            <v-img class="my_icon" src="../assets/images/design_i.png"></v-img>
            <h3>Web Design</h3>
        </div>

        <div class="box">
            <v-img class="my_icon" src="../assets/images/code_i.png"></v-img>
            <h3>Coding</h3>
        </div>

        <div class="box">
            <v-img class="my_icon" src="../assets/images/seo_i.png"></v-img>
            <h3>SEO</h3>
        </div>
    </div>
    </v-container>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>

    div.container {
        margin: auto auto;
    }

    .my-title {
        margin-top: 60px;
    }

    .box-wrap {
        margin: auto auto;
        width: 77vw;
        display: flex;
        justify-content: space-around;
        text-align: center;
        .box {
            width: 15vw;
            .my_icon {
                margin: auto auto;
                width: 50%;
            }
            h3 {
                color: white;
                padding-top: 30px;
            }
        }
    }

    @media only screen and (max-width: 700px) {
    .box-wrap {
        margin: auto auto;
        width: 77vw;
        display: flex;

        text-align: center;
        flex-flow: column;
        .box {
            margin: auto auto;
            width: 60vw;
            margin-bottom: 2vh;
            .my_icon {
                margin: auto auto;
                width: 45%;
            }
            h3 {
                color: white;
                padding-top: 30px;
            }
        }
    }
  }
</style>