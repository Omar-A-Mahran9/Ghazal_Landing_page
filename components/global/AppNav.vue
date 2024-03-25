<template>
  <nav class="navbar navbar-expand-lg">
    <div class="container-fluid d-flex justify-content-between">
      <a class="navbar-brand" href="#">
        <img src="/images/logo.svg" alt=""
      /></a>
      <div>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <nuxt-link class="nav-link" to="/#">{{
                $t("Join to us")
              }}</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link class="nav-link" to="/#">{{
                $t("Contact us")
              }}</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link class="nav-link" to="/#">{{
                $t("Download app")
              }}</nuxt-link>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
</template>
<style scoped>
.nav-link {
  color: white;
}
.navbar-toggler-icon {
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='white' stroke-linecap='round' stroke-miterlimit='100' stroke-width='3' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e");

  background-size: contain; /* Ensure the image fits within the button */
  width: 30px; /* Adjust width as needed */
  height: 20px; /* Adjust height as needed */
  display: inline-block; /* Ensure the button maintains proper size */
}
.navbar-toggler {
  border: 2px solid #ffff;
}
</style>
