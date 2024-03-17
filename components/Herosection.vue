<template>
  <v-container>
    <v-row no-gutters>
      <v-col cols="12" sm="12" md="6">
        <div class="main_container">
          <img
            class="fir-img"
            src="/images/Mobile/firstphone.svg"
            alt="First Phone Image"
            width="100%"
          />
          <img
            class="second-img"
            src="/images/Mobile/secondphone.svg"
            alt="Second Phone Image"
            width="100%"
          />
        </div>
      </v-col>
      <v-col cols="12" sm="12" md="6" class="main_container">
        <div>
          <h1 class="main_title mb-5">
            {{ $t("title1") }}
          </h1>
          <p id="sub-title" class="mb-5 pt-3">
            {{ $t("description1") }}
          </p>
        </div>

        <div class="store-icons pt-5">
          <!-- Google Play Store Icon with Link -->
          <a href="https://play.google.com/store">
            <img
              class="store-icon"
              src="/images/Play_Store.svg"
              alt="Google Play Store"
            />
          </a>

          <!-- Apple App Store Icon with Link -->
          <a href="https://apps.apple.com">
            <img
              class="store-icon"
              src="/images/App_Store.svg"
              alt="Apple App Store"
            />
          </a>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
<style scoped>
.main_container {
  position: relative;
}
.second-img {
  position: absolute;
  max-width: 61%;
  left: 18%;
}
.fir-img {
  position: absolute;
  max-width: 60%;
  right: 45%;
  top: 60px;
}

#sub-title {
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: 0em;
  text-align: right;
  color: white;
  margin-top: 10px;
  width: 89%;
  margin-left: 10%; /* Specify the margin from the left */
}
.store-icons {
  display: flex;
  gap: 10px;
  justify-content: flex-end; /* Align to the right */
}

.store-icon {
  width: 90%; /* Adjust as needed */
  cursor: pointer;
  margin-left: 10%; /* Specify the margin from the left */
}
/* Responsive styles based on screen size */
@media screen and (min-width: 768px) {
}

@media screen and (max-width: 960px) {
  .main_title {
    font-family: "Janna-Bold";
    font-size: 40px;
    font-weight: 700;
    line-height: 50px;
    letter-spacing: 1px;
    text-align: center;
    color: white;
  }
  .main_container {
    position: relative;
  }
  .second-img {
    position: absolute;
    max-width: 61%;
    left: 18%;
    display: none;
  }
  .fir-img {
    position: absolute;
    max-width: 60%;
    right: 45%;
    top: 60px;
    display: none;
  }

  #sub-title {
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    letter-spacing: 0em;
    text-align: center;
    color: white;
    margin-top: 10px;
    width: 89%;
    margin: auto; /* Specify the margin from the left */
  }
  .store-icons {
    display: flex;
    gap: 5px;
    justify-content: center;
    margin: auto;
  }

  .store-icon {
    width: 90%; /* Adjust as needed */
    cursor: pointer;
    margin-left: 10%;
  }
}

@media screen and (min-width: 1200px) {
}
</style>
