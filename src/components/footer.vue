<template>
  <div class="bg-black" style="width: 100vw; height: 50vh">
    <div
      class="q-mx-auto row q-pa-md"
      style="min-height: 50vh; max-width: 1140px"
    >
      <div class="col-12 text-grey-1 col-md-6 flex flex-center">
        <div class="q-pr-md" style="width: 100%">
          <div class="text-h3 q-my-md" style="font-weight: 700">
            <q-img
              src="~/src/assets/whitelogo.svg"
              alt="Menopause app graphic"
              class="q-mb-md"
              style="max-width: 150px"
            />
          </div>
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
      <div class="col-12 text-grey-1 col-md-6 flex flex-center">
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
</template>

<script setup>
import { ref } from "vue";
import heroSection from "src/components/hero.vue";
import funstats from "src/components/funstats.vue";
import Downloadapp from "src/components/downloadapp.vue";
import aboutsection from "src/components/aboutsection.vue";
import Aboutsection from "src/components/aboutsection.vue";
</script>
