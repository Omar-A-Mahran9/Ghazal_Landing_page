<template>
  <section class="">
    <div class="main-sec">
      <div class="d-flex justify-content-center container arrow-sec">
        <img class="arrow" src="/images/arrow.svg" alt="" />
      </div>
      <div class="custom-container container-fluid">
        <div class="d-flex justify-content-between align-items-center">
          <div class="d-flex flex-column">
            <img
              src="/images/locationicon.svg"
              width="100%"
              style="margin-bottom: 100px"
            />
            <img src="/images/papericon.svg" width="100%" />
          </div>
          <div class="d-flex flex-column">
            <div class="d-flex flex-column text-center mb-5">
              <h2 class="fw-bold mb-5">
                {{ $t("Download app") }}
                <span class="circle" style="color: #2d9596; padding: 4%">
                  {{ $t("now") }}
                </span>
              </h2>
              <p class="description">{{ $t("desc-main-sec") }}</p>
            </div>
            <div class="d-flex justify-content-center">
              <div class="store-icons pt-5">
                <!-- Google Play Store Icon with Link -->
                <a href="https://play.google.com/store">
                  <img
                    class="store-icon"
                    src="/images/Play_Store.svg"
                    alt="Google Play Store"
                    style="width: 90%; height: auto"
                  />
                </a>

                <!-- Apple App Store Icon with Link -->
                <a href="https://apps.apple.com">
                  <img
                    class="store-icon"
                    src="/images/App_Store.svg"
                    alt="Apple App Store"
                    style="width: 90%; height: auto"
                  />
                </a>
              </div>
            </div>
          </div>
          <div class="d-flex flex-column">
            <img
              src="/images/caricon.svg"
              width="100%"
              style="margin-bottom: 100px"
            />
            <img src="/images/tagicon.svg" width="100%" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.description {
  margin: auto;
  width: 70%;
}
.circle {
  background: url("/images/circle.svg") no-repeat center center;
  background-size: contain;
  padding: 10px; /* Adjust the padding as needed */
}
.main-sec {
  position: relative;
  height: 677px; /* Adjust based on your design needs */
  width: 100%; /* Ensure .main-sec spans the full width, adjust if necessary */
  margin-top: 200px;
}

.arrow-sec {
  position: absolute;
  left: 45%; /* Center horizontally */
  top: -7%; /* Center vertically */
  transform: translate(
    -50%,
    -50%
  ); /* Adjust position to truly center based on .arrow-sec dimensions */
}
.arrow {
  width: 10%;
}

.custom-container {
  display: flex;
  flex-direction: column;
  justify-content: center; /* Center content vertically */
  align-items: center; /* Center content horizontally */
  background-image: url("/images/Bg.svg"); /* Ensure correct path */
  height: 498px; /* Adjust based on your design needs */
  background-repeat: no-repeat;
  background-position: center; /* Center the background image */
  background-size: cover; /* Use 'cover' to fill the entire container, or 'contain' to fit the image into the container */
}
.store-icons {
  display: flex;
  gap: 20px;
}
p {
  line-height: 30px;
  color: #7689a1;
}
@media screen and (min-width: 992px) and (max-width: 1250px) {
}
@media screen and (min-width: 960px) and (max-width: 991px) {
}
@media screen and (max-width: 960px) {
  .description {
    margin: auto;
    width: 100%;
  }
  .main-sec {
    margin-top: 100px;
    height: 577px; /* Adjust based on your design needs */
  }

  .arrow-sec {
    position: absolute;
    left: 45%; /* Center horizontally */
    top: -1%; /* Center vertically */
    transform: translate(
      -50%,
      -50%
    ); /* Adjust position to truly center based on .arrow-sec dimensions */
  }
  .arrow {
    width: 4rem;
  }
}
@media screen and (max-width: 767px) {
}

@media screen and (min-width: 500px) {
}
</style>
