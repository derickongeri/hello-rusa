<template>
  <q-page class="flex">
    <div class="home-page" style="width: 100vw">
      <div
        class="hero-section q-ma-none q-pa-none"
        style="position: relative; max-width: 100vw"
      >
        <heroSection />
      </div>
      <!-- <div class="row items-center" style="min-height: 35vh">
        <funstats />
      </div> -->

      <div class="items-center q-mt-xl" style="min-height: 35vh">
        <Aboutsection />
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
      <div class="items-center q-mt-xl" style="min-height: 35vh">
        <appfeatures />
      </div>
      <div class="q-mt-lg hero-section" style="max-width: 100vw">
        <Downloadapp />
      </div>

      <!-- <Footer></Footer> -->
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
import appfeatures from "src/components/appfeatures.vue";
</script>

<style scoped>
.hero-section {
  background-color: #fbd2b4;
  max-width: 100vw;
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
