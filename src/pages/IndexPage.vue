<template>
  <q-page class="flex">
    <div class="home-page">
      <div class="bg-green-1" style="width: 100vw">
        <div
          class="row page-header items-center q-mx-xl"
          style="height: 10vh; margin: auto"
        >
          <div
            class="text-primary tabs-desktop text-h5"
            style="font-weight: 700"
          >
            Orusa
          </div>
          <div
            class="text-primary tabs-mobile q-ml-md text-h5"
            style="font-weight: 700"
          >
            Orusa
          </div>
          <q-space />
          <div class="tabs-desktop">
            <q-tabs no-caps align="left">
              <q-route-tab to="/page1" label="Press" />
              <q-route-tab to="/page2" label="Contact" />
              <q-route-tab to="/page3" label="Download" />
            </q-tabs>
          </div>
          <div class="tabs-mobile q-mr-sm">
            <q-btn flat round color="primary" icon="mdi-menu" />
          </div>
        </div>
        <heroSection />
        <!-- <div class="row q-mx-xl page-header" style="height: 80vh; margin: auto">
          <div class="col">
            <div
              class="column justify-center"
              style="height: 100%; width: 100%"
            >
              <div style="width: 90%">
                <div class="text-h3 q-my-md" style="font-weight: 700">
                  Manage Menopause with Confidence
                </div>
                <div class="text-h6 q-mb-md">
                  Some tagline to tell more about the app
                </div>
                <div class="q-mt-xl">
                  <q-btn
                    push
                    no-caps
                    color="black"
                    size="lg"
                    label="Get Started"
                  />
                </div>
              </div>
            </div>
          </div>
          <div class="col signup-page"></div>
        </div> -->
      </div>
      <div class="row items-center" style="width: 100vw; min-height: 35vh">
        <funstats />
      </div>
      <div class="text-center" style="width: 100vw">
        <div class="q-pa-md q-my-lg" style="max-width: 1140px; margin: auto">
          <q-video
            src="https://www.youtube.com/embed/af-356SbCkY?si=gz0jJpuDZ1DAxcnY"
            :ratio="16 / 9"
          />
        </div>
      </div>

      <div class="items-center q-mt-xl" style="width: 100vw; min-height: 35vh">
        <Aboutsection />
      </div>
      <div class="q-mt-lg" style="width: 100vw">
        <Downloadapp />
      </div>
      <div class="bg-black" style="width: 100vw; height: 50vh">
        <div
          class="q-mx-auto row q-pa-md"
          style="min-height: 50vh; max-width: 1140px"
        >
          <div class="col-12 text-grey-1 col-md-6 flex flex-center">
            <div class="q-pr-md" style="width: 100%">
              <div class="text-h3 q-my-md" style="font-weight: 700">Orusa</div>
              <div class="text-h6 q-mb-md">
                <div class="" style="max-width: 350px">
                  <q-list bordered separator>
                    <q-item clickable v-ripple>
                      <q-item-section>Press</q-item-section>
                    </q-item>
                    <q-item clickable v-ripple>
                      <q-item-section>Contact</q-item-section>
                    </q-item>
                    <q-item clickable v-ripple>
                      <q-item-section>Download</q-item-section>
                    </q-item>
                  </q-list>
                </div>
              </div>
              <div class="q-mt-xl">
                <q-btn
                  push
                  no-caps
                  color="black"
                  size="lg"
                  label="Get Started"
                  @click="navigateToSignup"
                />
              </div>
            </div>
          </div>
          <div
            class="col-12 text-grey-1 col-md-6 flex flex-center"
          >
            <div>
              <!-- Add an image or graphic for visual appeal -->
              <div class="text-h5 q-my-md" style="font-weight: 700">
                Join our Community
              </div>

              <div>
                <q-input
                  dark
                  outlined
                  standout
                  v-model="text"
                  style="border-radius: 20px; width: 100%"
                  class=""
                >
                  <template v-slot:append>
                    <q-btn
                      style="width: 150px"
                      class="q-ml-md"
                      push
                      label="Subscribe"
                      no-caps
                      size="lg"
                      color="grey-1"
                      text-color="grey-9"
                    />
                  </template>
                </q-input>
              </div>
            </div>
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
</script>

<style scoped>
.my-card {
  max-width: 600px;
  margin: 0 auto;
}

.q-page {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
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
