<template>
  <!-- About Section -->
  <div class="about-section q-py-md">
    <div class="q-mb-md">
      <!-- Centered Title -->
      <div class="text-h3 header-text text-center q-mb-lg" style="">
        About Orusa
      </div>
    </div>

    <!-- Body Text -->
    <div class="text-body1 q-pa-md text-justify caption-text">
      <p>
        At Orusa App, we are proud to introduce the first African menopause app,
        created to address the unique needs of women experiencing menopause
        across the continent. Menopause is a natural stage in a woman’s life,
        yet it is often misunderstood and under-discussed, especially within
        African communities. Our mission is to break the silence, provide
        accurate information, and create a supportive space for women to
        navigate this life transition with confidence.
      </p>

      <p>
        Orusa app offers tailored resources, expert advice, and a supportive
        community to help women understand and manage the physical, emotional,
        and mental changes that come with menopause. From personalized symptom
        tracking to practical tips on nutrition, exercise, and mental
        well-being, Orusa App empowers African women to embrace their menopause
        journey.
      </p>

      <p>
        With a focus on cultural relevance, inclusivity, and comprehensive
        support, we aim to elevate the conversation around menopause in Africa,
        providing women with the tools they need to thrive during this life
        stage. Whether you’re just beginning your menopause journey or
        navigating the various stages, Orusa App is here to guide, educate, and
        support you every step of the way.
      </p>
    </div>
  </div>

  <!--

  <div class="app-features">

    <div class="features-section q-pa-md">

      <div class="q-gutter-x-xl row justify-center">

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
              <div class="text-center" style="max-width: 300px; margin: auto">
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
              src="~/src/assets/mockup1.png"
              alt="Menopause app graphic"
              class="q-mb-md"
              style="max-width: 80%"
            />
            <q-card-section>
              <div class="text-center" style="max-width: 300px; margin: auto">
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
              <div class="text-center" style="max-width: 300px; margin: auto">
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
              <div class="text-center" style="max-width: 300px; margin: auto">
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

  -->
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
