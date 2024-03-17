<template>
  <section class="pt-5 mb-5" dir="rtl">
    <div class="last-section container back">
      <div class="row content-div">
        <div class="col-md-6 col-12 p-5 form">
          <div>
            <form id="contact_form" name="contact_form" method="post">
              <div class="col">
                <input
                  type="text"
                  required
                  maxlength="100"
                  :placeholder="$t('Name')"
                  class="form-control"
                  id="name"
                  name="name"
                />
              </div>
              <div class="col">
                <input
                  type="text"
                  required
                  maxlength="50"
                  :placeholder="$t('Garage Name')"
                  class="form-control"
                  id="garage_name"
                  name="garage_name"
                />
              </div>
              <div class="col">
                <input
                  type="text"
                  required
                  maxlength="50"
                  class="form-control"
                  :placeholder="$t('Phone')"
                  id="phone_input"
                  name="Phone"
                />
              </div>
              <div class="mb-5">
                <textarea
                  class="form-control"
                  id="message"
                  name="message"
                  rows="5"
                  :placeholder="$t('Message')"
                ></textarea>
              </div>
              <div>
                <input
                  class="form-check-input ml-4"
                  type="checkbox"
                  value=""
                  id="approveCheckbox"
                  style="width: 20px; height: 20px"
                />
                <label class="form-check-label" for="approveCheckbox">
                  {{ $t("Approved") }}
                </label>
              </div>
              <button
                type="submit"
                class="btn d-flex align-items-center justify-content-between"
                style="width: 205px; color: white"
              >
                <div class="m-1">
                  {{ $t("Send") }}
                </div>
                <div>
                  <span><img src="/images/arrow-left.svg" alt="" /></span>
                </div>
              </button>
            </form>
          </div>
        </div>
        <div class="col-md-6 col-12 rightsection">
          <h1 class="mb-5 fw-bold text-light">
            {{ $t("description last section") }}
          </h1>
          <p class="text-light">{{ $t("subdescription") }}</p>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
input {
  margin-bottom: 20px;
  height: 60px;
  border-radius: 8px;
}
.form {
  background-color: white;
  border-radius: 25px;
  width: 546px;
  box-shadow: 0px 80.5999984741211px 105.70134735107422px 0px #3333331a;
}
input:focus {
  border: black;
  margin-bottom: 14px;
}
button {
  background: linear-gradient(247.15deg, #2d9596 130.42%, #3cadae 1021.43%);
  color: white;
}
.form-check-input:checked {
  background-color: #2c9596;
  border-color: #2c9596;
}
.back {
  height: 100%;
  background-color: #2d9596; /* Background color of the shape */
  border-radius: 25px; /* Border radius to create rounded corners */
  z-index: -1;
}

.content-div {
  z-index: 1;
}
.rightsection {
  padding-right: 80px;
  width: 40%;
  margin: auto;
  margin-right: 0;
  line-height: 30px;
}
</style>
