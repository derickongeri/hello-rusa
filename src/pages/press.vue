<template>
  <q-page class="flex">
    <div class="home-page" style="width: 100vw;">
      <div class="row items-center justify-center" style="width: 100vw; min-height: 15vh;">
      <div class="header-text text-h3 text-center q-my-lg" style="font-weight: 700">
        Press
      </div>
    </div>
      <div class="text-center" style="width: 100%">
        <div class="q-pa-md q-my-lg" style="max-width: 1140px; margin: auto">
          <div class="q-video">
            <iframe
              src="https://player.cloudinary.com/embed/?public_id=WhatsApp_Video_2025-01-09_at_10.59.59_sqkg9b&cloud_name=dv3id0zrx&profile=cld-defaul"
              width="640"
              height="360"
              style="height: auto; width: 100%; aspect-ratio: 640 / 360"
              allow="autoplay; fullscreen; encrypted-media; picture-in-picture"
              frameborder="0"
              allowfullscreen
            />
          </div>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script setup>
import { ref } from "vue";
import heroSection from "src/components/hero.vue";
import funstats from "src/components/funstats.vue";
import Downloadapp from "src/components/downloadapp.vue";
import aboutsection from "src/components/aboutsection.vue";
import Aboutsection from "src/components/aboutsection.vue";
import Footer from "src/components/footer.vue";
</script>

<style scoped>
.hero-section {
  background-color: #fbd2b4;
}

.my-card {
  max-width: 600px;
  margin: 0 auto;
}

.q-page {
  display: flex;
  align-items: center;
  justify-content: center;
}

.page-header {
  max-width: 1140px;
}

.signup-page {
  /* Set the background image and ensure it covers the entire element */
  background-image: url("~/src/assets/img3.jpg"); /* Adjust the path as per your project structure */
  background-size: cover;
  background-position: center;
}
</style>
