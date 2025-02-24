<template>
  <!-- Header Section -->
  <div
    class="q-mx-auto row"
    style="min-height: 50vh; max-width: 1400px"
  >
    <div class="col-12 col-md-6 flex flex-center">
      <div class="q-pr-md q-ma-xl" style="width: 100%">
        <div class="text-h3 q-my-md" style="font-weight: 700">
          Download OrusaApp
        </div>
        <div class="text-h6 q-mb-md">Available for both Android and iOS Devices</div>
        <div class="q-mt-xl">
          <div class="row q-gutter-x-md items-center">
            <a href="">
              <div style="width: 250px" class="ios-btn"></div>
            </a>

            <a href="">
              <div style="width: 250px" class="android-btn"></div>
            </a>
          </div>
        </div>
      </div>
    </div>
    <div class="col-12 col-md-6 flex flex-center tabs-desktop">
      <!-- Add an image or graphic for visual appeal -->
      <q-img
        src="~/src/assets/2.svg"
        alt="Menopause app graphic"
        class="q-mb-"
        style="max-width: 100%"
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
  background-image: url("~/src/assets/googleplay.svg");
  background-size: cover; /* Ensures the SVG covers the entire div */
  background-position: center; /* Centers the SVG */
  background-repeat: no-repeat; /* Prevents the SVG from repeating */
}

.ios-btn {
  width: 100%;
  height: 70px; /* Adjust the height based on your needs */
  background-image: url("~/src/assets/appstore.svg");
  background-size: cover; /* Ensures the SVG covers the entire div */
  background-position: center; /* Centers the SVG */
  background-repeat: no-repeat; /* Prevents the SVG from repeating */
}

.q-page {
  height: 100vh; /* Ensures the page fills the screen */
}
</style>
