<template>
  <v-content>
    <div class="staticHero">
      <v-img src="../assets/images/396602.jpg">
      <v-row align="end" class="lightbox white--text pa-2 fill-height">
        <v-col>
          <v-container>
            <!-- <div class="headline">Contact Me</div> -->
          </v-container>
        </v-col>
      </v-row>
    </v-img>
    </div>
    <div class="block my_block">
      <div class="my_form">
        <h2 style="font-size: 40px;">Drop me a line</h2>
        <h3>I would love to hear from you</h3>
        <p>Would you like to discuss a potential project? maybe you just want to stop in and say hi?
          you can send me a message using the contact form, or reach me using the information below </p>
          <hr />
          <h4>Contact information:</h4>
          <p><span>E-mail:  </span>pwinston@gmail.com</p>
          <p><span></span></p>
      </div>

      <div class="my_form">
        <v-form ref="form" v-model="valid" lazy-validation>
          <v-text-field class="my_txt" v-model="name" :counter="10" :rules="nameRules" label="Name" required></v-text-field>
          <v-text-field class="my_txt" v-model="email" :rules="emailRules" label="E-mail" required></v-text-field>
          <v-text-field class="my_txt" label="Number" required></v-text-field>
          <v-textarea class="my_txt" v-model="message" :rules="messageRules" label="Message" required></v-textarea>
          <v-btn :disabled="!valid" color="#2c399e" class="mr-4 my_btn" @click="validate">Send</v-btn>
          <!-- <v-btn color="error" class="mr-4" @click="reset">Reset</v-btn> -->
        </v-form>
      </div>
    </div>
    <div class="googlemap">
      <!-- <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d16705.802661855836!2d-0.14290489950731525!3d51.50711704027593!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47d8a00baf21de75%3A0x52963a5addd52a99!2sLondon!5e0!3m2!1sen!2suk!4v1577041400110!5m2!1sen!2suk" width="100%" height="450"></iframe> -->
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2260.5403274101823!2d8.443174915907628!3d55.488109180483434!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x464b20dde4535e3f%3A0xb1611bd698540663!2sSpangsbjerg%20Kirkevej%20105%2C%206700%20Esbjerg!5e0!3m2!1sda!2sdk!4v1620371853874!5m2!1sda!2sdk" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
    </div>
  </v-content>
</template>

<script>
export default {
  name: "Contact",
  data: () => ({
    valid: true,
    name: "",
    nameRules: [
      v => !!v || "Name is required",
      v => (v && v.length <= 10) || "Name must be less than 10 characters"
    ],
    email: "",
    emailRules: [
      v => !!v || "E-mail is required",
      v => /.+@.+\..+/.test(v) || "E-mail must be valid"
    ],
    message: "",
    messageRules: [
      v => !!v || "Message is required",
      v => (v && v.length >= 10) || "Message must be more than 10 characters"
    ],
  }),

  methods: {
    validate() {
      if (this.$refs.form.validate()) {
        this.snackbar = true;
      }
    },
    reset() {
      this.$refs.form.reset();
    }
  }
};
</script>

<style lang="scss">

  .my_block {
    display: flex;
    justify-content: space-around;
    text-align: center;

    h2 {
      color: 	#2c399e;
      font-weight: 900;
      height: 60px;
      
    }

    h3 {
      color: #747474;
      margin-top: -6%;
    }

    h4 {
      color: white;
      padding-top: 5%;
    }

    p {
      color: white;
      padding-bottom: 5%;
    }
  }

  .my_form {
    width: 45vw;
    background-color: black;

    .my_btn {
      width: 100%;
      color: white;
    }
  }

  .my_txt {
    color: green;
  }

  input, textarea {
    background-color: #e2e2e2;
    border-radius: 5px;
    padding: 10px;
    
  }

  @media only screen and (max-width: 700px) {
    .my_block {
        display: flex;
        justify-content: space-around;
        text-align: center;
        flex-flow: column;

        h2 {
          color: 	#2c399e;
          font-weight: 900;
          height: 60px;
        }

        h3 {
          color: #747474;
          margin-top: -4vh;
        }

          .my_form {
          margin: auto auto;
          width: 90vw;
          background-color: black;
          margin-bottom: 2vh;

        .my_btn {
          width: 100%;
        }
      }
    }
  }
  
</style>