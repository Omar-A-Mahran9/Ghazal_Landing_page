<template>
  <section class="container" dir="rtl">
    <div class="row setion5">
      <div class="col-12 sec1">
        <div class="about-us">
          <p>{{ $t("about-us") }}</p>
        </div>
        <div class="image-container">
          <img src="/images/Macbook.png" alt="" class="macbook-img" />
          <img src="/images/mobile.png" alt="" class="mobile-img" />
        </div>
      </div>
      <div class="col-12 sec2">
        <div class="row">
          <div class="col-lg-4 col-12 mb-5">
            <div class="column-content">
              <div class="d-flex align-items-center gap-5">
                <div>
                  <img src="/images/1icon.svg" alt="" />
                </div>
                <div>
                  <p class="title-icons">{{ $t("first-title") }}</p>
                  <p class="description-icons">{{ $t("first-description") }}</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-4 col-12 mb-5">
            <div class="column-content">
              <div class="d-flex align-items-center gap-5">
                <div>
                  <img src="/images/2dicon.svg" alt="" />
                </div>
                <div>
                  <p class="title-icons">{{ $t("secound-title") }}</p>
                  <p class="description-icons">
                    {{ $t("secound-description") }}
                  </p>
                </div>
              </div>
            </div>
          </div>
          <div class="col-lg-4 col-12">
            <div class="column-content">
              <div class="d-flex align-items-center gap-5">
                <div>
                  <img src="/images/3dicon.svg" alt="" />
                </div>
                <div>
                  <p class="title-icons">{{ $t("third-title") }}</p>
                  <p class="description-icons">
                    {{ $t("third-description") }}
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.section5 {
}
.about-us {
  width: 60%;
  text-align: center;
  margin: auto;
  font-size: 24px;
}
.image-container {
  position: relative;
  margin-top: 50px;
  height: 659px !important;
}

.column-content {
  width: 90%; /* Makes the content occupy 90% of the column width */
  margin: auto; /* Centers the content within the column */
}
.macbook-img,
.mobile-img {
  width: 100%;
  position: absolute;
}

.macbook-img {
  z-index: 1;
  top: 0;
  left: 0;
}

.mobile-img {
  z-index: 2;
  width: 25%;
  top: 40%;
  right: 9%;
}
.title-icons {
  font-weight: bold;
}
.description-icons {
  text-align: justify;
}
.sec2 {
  margin-top: 140px;
}
.description-icons {
  color: #888;
}
@media screen and (min-width: 992px) and (max-width: 1250px) {
  .mobile-img {
    z-index: 2;
    top: 12rem;
    right: 6rem;
  }
  .sec2 {
    margin-top: -10px;
  }
}
@media screen and (min-width: 960px) and (max-width: 991px) {
  .mobile-img {
    z-index: 2;
    top: 7.5rem;
    right: 4rem;
  }
  .sec2 {
    margin-top: -180px;
  }
}
@media screen and (max-width: 960px) {
  .about-us {
    width: 90%;
    text-align: center;
    margin: auto;
    font-size: 1.3rem;
  }
  .mobile-img {
    z-index: 2;
    top: 7.5rem;
    right: 4rem;
  }
  .image-container {
    position: relative;
    margin-top: 50px;
    height: 300px !important;
  }
  .column-content {
    width: 80%; /* Makes the content occupy 90% of the column width */
  }
  .sec2 {
    margin-top: 130px;
  }
}
@media screen and (max-width: 767px) {
  .mobile-img {
    z-index: 2;
    top: 5.8rem;
    right: 2.7rem;
  }
  .about-us {
    width: 90%;
    text-align: center;
    margin: auto;
    font-size: 17px;
  }
  .sec2 {
    margin-top: 50px;
  }
}

@media screen and (max-width: 500px) {
  .mobile-img {
    z-index: 2;
    top: 4rem;
    right: 2rem;
  }
}
</style>
