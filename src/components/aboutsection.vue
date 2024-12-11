<template>
  <!-- About Section -->
  <div class="about-section q-pa-md">
    <div class="q-mb-md">
      <!-- Centered Title -->
      <div class="text-h3 text-center q-mb-lg" style="font-weight: 700">
        Orusa is making a difference
      </div>
    </div>

    <!-- Body Text -->
    <div class="text-body1 caption-text text-center">
      Orusa is a comprehensive app designed to empower women through the
      menopause journey. With features like sign tracking, expert advice, and
      community insights, our goal is to help you navigate menopause with
      confidence. We are here to support you every step of the way.

      <br /><br />

      Join thousands of women who are taking control of their health with Orusa.
    </div>
  </div>

  <div class="app-features">
    <!-- Features Section -->
    <div class="features-section q-pa-md">
      <!-- Grid Layout: Two Columns on Larger Screens, One Column on Mobile -->
      <div class="q-gutter-x-xl row justify-center">
        <!-- Feature 1 -->
        <div class="col-12 col-md-4">
          <q-card flat class="feature-card" shadow="2">
            <q-img
              src="https://via.placeholder.com/400"
              alt="Feature 1 Illustration"
              class="q-mb-md"
              height="578px"
              contain
            />
            <q-card-section>
              <div class="text-center" style="max-width: 300px;margin: auto;">
                <div class="text-h6 text-center head-text q-mb-sm">
                  App Feature
                </div>
                <div class="text-body2 caption-text text-center">
                  Some text giving an explanation to the app feature captured
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>

        <div class="col-12 col-md-4">
          <q-card flat class="feature-card" shadow="2">
            <q-img
              src="https://via.placeholder.com/400"
              alt="Feature 1 Illustration"
              class="q-mb-md"
              height="578px"
              contain
            />
            <q-card-section>
              <div class="text-center" style="max-width: 300px;margin: auto;">
                <div class="text-h6 text-center head-text q-mb-sm">
                  App Feature
                </div>
                <div class="text-body2 caption-text text-center">
                  Some text giving an explanation to the app feature captured
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>

        <div class="col-12 col-md-4">
          <q-card flat class="feature-card" shadow="2">
            <q-img
              src="https://via.placeholder.com/400"
              alt="Feature 1 Illustration"
              class="q-mb-md"
              height="578px"
              contain
            />
            <q-card-section>
              <div class="text-center" style="max-width: 300px;margin: auto;">
                <div class="text-h6 text-center head-text q-mb-sm">
                  App Feature
                </div>
                <div class="text-body2 caption-text text-center">
                  Some text giving an explanation to the app feature captured
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>

        <div class="col-12 col-md-4">
          <q-card flat class="feature-card" shadow="2">
            <q-img
              src="https://via.placeholder.com/400"
              alt="Feature 1 Illustration"
              class="q-mb-md"
              height="578px"
              contain
            />
            <q-card-section>
              <div class="text-center" style="max-width: 300px;margin: auto;">
                <div class="text-h6 text-center head-text q-mb-sm">
                  App Feature
                </div>
                <div class="text-body2 caption-text text-center">
                  Some text giving an explanation to the app feature captured
                </div>
              </div>
            </q-card-section>
          </q-card>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
</script>

<style scoped>
.about-section {
  max-width: 1140px; /* Limit the width for larger screens */
  margin: 0 auto; /* Center the section */
}

.app-features {
  width: 100vw;
}

.features-section {
  margin: 0 auto; /* Center the section */
}

.feature-card {
  margin: 10px;
  /* Customize card styling if needed */
  border-radius: 12px; /* Rounded corners */
}

.q-page {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}

.text-center {
  text-align: center;
}

.head-text {
  font-weight: 700;
}

.caption-text {
  font-size: large;
}
</style>
