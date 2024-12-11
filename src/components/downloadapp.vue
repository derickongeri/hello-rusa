<template>
  <!-- Header Section -->
  <div
    class="q-mx-auto bg-green-1 row q-pa-lg"
    style="min-height: 50vh; max-width: 1400px"
  >
    <div class="col-12 col-md-6 flex flex-center">
      <div class="q-pr-md q-ma-xl" style="width: 100%">
        <div class="text-h3 q-my-md" style="font-weight: 700">
          You're not alone in your journey.
        </div>
        <div class="text-h6 q-mb-md">Get the app for free</div>
        <div class="q-mt-xl">
          <div class="row q-gutter-x-md items-center">
            <q-btn
              push
              no-caps
              flat
              color=""
              size="lg"
              label=""
              @click="navigateToSignup"
              style="width:250px"
            >
            <div class="ios-btn"></div>
          </q-btn>
            <q-btn
              push
              no-caps
              flat
              color=""
              size="lg"
              label=""
              @click="navigateToSignup"
              style="width:250px"
            >
            <div class="android-btn"></div>
          </q-btn>
          </div>
        </div>
      </div>
    </div>
    <div class="col-12 col-md-6 flex flex-center tabs-desktop">
      <!-- Add an image or graphic for visual appeal -->
      <q-img
        src="https://via.placeholder.com/400"
        alt="Menopause app graphic"
        class="q-mb-md"
        style="max-width: 80%"
      />
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import { useRouter } from "vue-router";

const router = useRouter();

function navigateToSignup() {
  // Example of navigating to a signup or intro page (modify as needed)
  router.push("/signup");
}
</script>

<style scoped>
/* You can adjust the max-width and height of your page as needed */
.page-header {
  display: flex;
  justify-content: center;
  align-items: center;
}

.signup-page {
  background-color: #f5f5f5; /* Add a background color if you want */
  display: flex;
  justify-content: center;
  align-items: center;
}

.android-btn {
  width: 100%;
  height: 100px; /* Adjust the height based on your needs */
  background-image: url('~/src/assets/googleplay.svg');
  background-size: cover; /* Ensures the SVG covers the entire div */
  background-position: center; /* Centers the SVG */
  background-repeat: no-repeat; /* Prevents the SVG from repeating */
}

.ios-btn {
  width: 100%;
  height: 70px; /* Adjust the height based on your needs */
  background-image: url('~/src/assets/appstore.svg');
  background-size: cover; /* Ensures the SVG covers the entire div */
  background-position: center; /* Centers the SVG */
  background-repeat: no-repeat; /* Prevents the SVG from repeating */
}

.q-page {
  height: 100vh; /* Ensures the page fills the screen */
}
</style>
