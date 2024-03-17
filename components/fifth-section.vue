<template>
  <section class="container" dir="rtl">
    <div class="row">
      <div class="col-12">
        <div
          style="width: 60%; text-align: center; margin: auto; font-size: 24px"
        >
          <p>{{ $t("about-us") }}</p>
        </div>
        <div class="image-container">
          <img src="/images/Macbook.png" alt="" class="macbook-img" />
          <img src="/images/mobile.png" alt="" class="mobile-img" />
        </div>
      </div>
      <div class="col-12">
        <div class="row">
          <div class="col-md-3 col-12">
            <div>
              <div></div>
              <div></div>
            </div>
          </div>
          <div class="col-md-3 col-12"></div>
          <div class="col-md-3 col-12"></div>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.image-container {
  position: relative;
  height: 659px;
  margin-top: 50px;
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
  top: 230px;
  right: 90px;
}
</style>
