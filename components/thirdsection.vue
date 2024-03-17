<template>
  <v-container>
    <v-row no-gutters>
      <v-col cols="12" sm="6"> </v-col>
      <v-col cols="12" sm="6">
        <div>
          <div class="text_container">
            <span class="sub_title">{{ $t("section3span") }}</span>
            <p class="tiltle">{{ $t("why Ghazell") }}</p>
            <p class="description">{{ $t("description2") }}</p>
          </div>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
<style>
.text_container {
  text-align: right;
  width: 474px;
}
.sub_title {
  font-size: 14px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: 0px;
  color: #2d9596;
}
.tiltle {
  font-family: "Janna-Bold";
  font-size: 40px;
  font-weight: 700;
  letter-spacing: 0px;
  text-align: right;
}
.description {
font-size: 20px
;
}
</style>
