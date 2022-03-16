<template>
  <div>
    <v-layout>
      <v-container>
        <div class="navbar">
          See how you can build this app
          <a href="https://www.youtube.com/1manstartup">here</a>
        </div>
      </v-container>
    </v-layout>
    <v-layout class="middle">
      <v-container>
        <v-row class="cont">
          <v-col class="d-flex justify-center" cols="12" md="6">
            <img class="img" src="../assets/Travel.png" />
          </v-col>
          <v-col cols="12" md="6">
            <div class="card1">
              <div class="tex1">Travel Treasury</div>
              <div class="tex2">Budget For Your Next Adventure</div>
              <h5 class="h5">Download For Free</h5>
              <v-row>
                <v-col cols="6" md="6">
                  <a
                    href="https://apps.apple.com/us/app/travel-treasury/id1534464018"
                  >
                    <img
                      style="padding: 2%"
                      height="95px"
                      width="100%"
                      src="../assets/Apple.png"
                    />
                  </a>
                </v-col>
                <v-col cols="6" md="6">
                  <a
                    href="https://play.google.com/store/apps/details?id=com.a1manstartup.travel_budget_first"
                  >
                    <img width="100%" src="../assets/Google.png" />
                  </a>
                </v-col>
              </v-row>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-layout>
    <v-layout mt-7>
      <v-container>
        <v-row>
          <v-col class="d-flex justify-center" cols="12" md="4">
            <img width="50%" height="400px" src="../assets/Iphone1.png" />
          </v-col>
          <v-col class="d-flex justify-center" cols="12" md="4">
            <img width="50%" height="400px" src="../assets/Iphone2.png" />
          </v-col>
          <v-col class="d-flex justify-center" cols="12" md="4">
            <img width="50%" height="400px" src="../assets/Iphone3.png" />
          </v-col>
        </v-row>
      </v-container>
    </v-layout>
    <v-layout>
      <v-container>
        <v-row>
          <v-col cols="12" md="4">
            <h4 class="text-center">PLAN</h4>
            <h5 class="text-center">
              Plan your next adventure by setting a daily spending budget. We
              make it easy to break your expenses down by category, giving you
              more time to plan the important things!
            </h5>
          </v-col>
          <v-col cols="12" md="4">
            <h4 class="text-center">SAVE</h4>
            <h5 class="text-center">
              Use the app to track how much money you've saved towards your
              trips total budgeted goal. Know exactly how much more you need to
              save, and how much time you have left to save.
            </h5>
          </v-col>
          <v-col cols="12" md="4">
            <h4 class="text-center">BUDGET</h4>
            <h5 class="text-center">
              When the day of your trip comes, have the peace of mind that you
              planned out your expenses. Never worry about money on a trip
              again!
            </h5>
          </v-col>
        </v-row>
      </v-container>
    </v-layout>
    <v-layout class="last">
      <v-container>
        <v-row>
          <v-col class="text-center" cols="12" md="12">
            <h2 class="h2">Have Any Questions?</h2>
            <p class="p">Contact us by filling out the information below</p>
            <form>
              <input
                v-model.trim="$v.email.$model"
                class="box"
                type="text"
                placeholder="Enter Your Email"
              />
              <div class="error1" v-if="!$v.email.required">
                Email is required
              </div>

              <v-textarea
                class="area"
                background-color="white"
                color="black"
                label="Enter Your Message"
              ></v-textarea
              ><br />
              <button class="btn">Send Message</button>
            </form>
            <h5 class="h55">Download For Free</h5>
            <v-row>
              <v-col cols="6" md="6">
                <a
                  href="https://apps.apple.com/us/app/travel-treasury/id1534464018"
                >
                  <img
                    style="padding: 2%"
                    width="300px"
                    height="100px"
                    src="../assets/AppSTORE.png"
                  />
                </a>
              </v-col>
              <v-col cols="6" md="6">
                <a
                  href="https://play.google.com/store/apps/details?id=com.a1manstartup.travel_budget_first"
                >
                  <img
                    width="300px"
                    height="88px"
                    src="../assets/GogglePLay.png"
                  />
                </a>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-container>
    </v-layout>
    <v-layout style="background-color: black">
      <v-container>
        <v-row>
          <v-col class="text-center" cols="12" md="12">
            <a class="a1" href="https://www.youtube.com/"
              >Build This App || By Darshan</a
            >
          </v-col>
        </v-row>
      </v-container>
    </v-layout>
  </div>
</template>

<script>
import { required } from "vuelidate/lib/validators";
export default {
  data() {
    return {
      email: "",
    };
  },
  validations: {
    email: {
      required,
    },
  },

};
</script>
<style scoped>
.navbar {
  text-align: center;
  color: #818182;
  background-color: #fefefe;
  border-color: #fdfdfe;
}
.middle {
  background: url(../assets/background-image.jpeg);
  background-size: cover;
  height: 500px;
}
.img {
  max-height: 80vh;
  width: 35%;
}
.cont {
  padding: 5%;
}
.card1 {
  height: 303px;
  width: 570px;
  background-color: white;
}
.tex1 {
  color: #3f51b5;
  font-size: 55px;
  text-align: center;
}
.tex2 {
  color: #3f51b5;
  font-size: 30px;
  text-align: center;
}
.h5 {
  color: #6c757d !important;
  text-align: center;
  font-size: 1.25rem;
  font-weight: 400;
}
h4 {
  color: #3f51b5;
  font-size: 1.5rem;
}
h5 {
  font-size: 1.25rem;
  color: #818182;
}
a {
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}
.last {
  background-color: #3f51b5;
}
.h2 {
  font-size: 2rem;
  font-weight: 400;
  color: whitesmoke;
}
.p {
  color: whitesmoke;
}
.box {
  background-color: white;
  width: 428px;
  height: 38px;
}
.area {
  height: 134px;
  width: 428px;
  left: 0;
  right: 0;
  margin: auto;
}
.btn {
  background-color: white;
  padding: 6px;
  color: black;
}
.h55 {
  margin-top: 5%;
  font-size: 20px;
  color: white;
  font-weight: 400;
}
.a1 {
  color: orange;
}
.a1:hover {
  text-decoration: none;
}
.error1{
  color: yellow;
}
</style>
