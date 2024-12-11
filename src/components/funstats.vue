<template>
  <div class="q-mx-auto row q-gutter-y-lg q-pa-md">
    <!-- Desktop Layout: 3 Columns (col-md-4) and Mobile Layout: 1 Column (col-12) -->
    <div class="col-12 col-md-4">
      <q-card flat class="my-card" shadow="2">
        <q-card-section>
          <div class="text-h5 text-center head-text q-mb-sm">85% of women</div>
          <div class="caption-text text-center">
            Experience signs of menopause.
          </div>
        </q-card-section>
      </q-card>
    </div>

    <div class="col-12 col-md-4">
      <q-card flat class="my-card" shadow="2">
        <q-card-section>
          <div class="text-h5 text-center head-text q-mb-sm">70% of women</div>
          <div class="caption-text text-center">
            Say menopause impacts their daily life
          </div>
        </q-card-section>
      </q-card>
    </div>

    <div class="col-12 col-md-4">
      <q-card flat class="my-card" shadow="2">
        <q-card-section>
          <div class="text-h5 text-center head-text q-mb-sm">60% of women</div>
          <div class="caption-text text-center">
            Feel isolated in their journey
          </div>
        </q-card-section>
      </q-card>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
</script>

<style scoped>
.my-card {
  margin: 10px;
  /* Add some custom styling to your card if needed */
  max-width: 100%;
}

.head-text{
  font-weight: 700;
}

.caption-text {
  font-size: large;
}
</style>
