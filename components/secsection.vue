<template>
  <section class="container">
    <div
      class="d-flex flex-column justify-content-center align-items-center w-100 text-center"
    >
      <p class="main_title text-dark" style="font-size: 40px">
        {{ $t("About Gazell") }}
      </p>
      <p class="description">{{ $t("description") }}</p>
    </div>

    <div class="video-container">
      <div class="play-button" data-video-id="YOUR_VIDEO_ID">
        <div class="thumbnail-overlay"></div>
        <img
          class="thumbnail-image"
          src="/images/illustration.svg"
          alt="Video Thumbnail"
          wi
        />
        <div class="play-icon"></div>
      </div>
      <div class="youtube-player">
        <iframe
          width="100%"
          height="100%"
          :src="videoUrl"
          frameborder="0"
          allowfullscreen
        ></iframe>
      </div>
    </div>
  </section>
</template>
<script setup>
import { ref } from "vue";

const showPlayer = ref(false);
const videoUrl = ref("");

const playVideo = () => {
  const videoId = document
    .querySelector(".play-button")
    .getAttribute("data-video-id");
  videoUrl.value = `https://www.youtube.com/embed/TCZNX5p6u9g?si=U4d1KTb8SRqcflhf`;
  showPlayer.value = true;
};
</script>

<style scoped>
.description {
  font-size: 20px;
  font-weight: 400;
  line-height: 32px;
  letter-spacing: 0em;
  text-align: center;
  color: #7689a1;
  width: 44%;
  margin-bottom: 60px;
}
.video-container {
  position: relative;
  width: 100%;
  height: 100%;
  margin: 0 auto;
  border-radius: 24px;
}

.play-button {
  position: relative;
  display: block;
  width: 100%;
  overflow: hidden;
  cursor: pointer;
  z-index: 99;
}

.play-button img {
  width: 100%;
  height: auto;
}

.play-icon {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 80px; /* Adjust the size of the play button */
  height: 80px; /* Adjust the size of the play button */
  background: url("/images/play.svg") no-repeat center center;
  background-size: contain;
  z-index: 99999999;
}

.youtube-player {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
.youtube-player iframe {
  border-radius: 24px;
}
.thumbnail-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 24px;
  background: #22272e;
  opacity: 0.64;
  z-index: 9;
}
.thumbnail-image {
  width: 50% !important;
  display: block;
  margin: auto;
  padding: 100px;
}
@media screen and (max-width: 959px) {
  .description {
    font-size: 16px;
    font-weight: 400;
    line-height: 32px;
    letter-spacing: 0em;
    text-align: center;
    color: #7689a1;
    width: 90%;
  }
}
</style>
