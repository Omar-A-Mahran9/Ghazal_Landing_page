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
</style>
