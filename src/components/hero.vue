<template>
    <!-- Header Section -->
    <div class="q-mx-auto row q-pa-md" style="min-height: 50vh;max-width: 1140px;">
      <div class="col-12 col-md-6 flex flex-center">
        <div class="q-pr-md" style="width: 100%;">
          <div class="text-h3 q-my-md" style="font-weight: 700;">
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
              @click="navigateToSignup"
            />
          </div>
        </div>
      </div>
      <div class="col-12 col-md-6 flex flex-center tabs-desktop">
        <!-- Add an image or graphic for visual appeal -->
        <q-img
          src="https://via.placeholder.com/400"
          alt="Menopause app graphic"
          class="q-mb-md"
          style="max-width: 80%;"
        />
      </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import { useRouter } from 'vue-router';

const router = useRouter();

function navigateToSignup() {
  // Example of navigating to a signup or intro page (modify as needed)
  router.push('/signup');
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

.q-page {
  height: 100vh; /* Ensures the page fills the screen */
}
</style>
