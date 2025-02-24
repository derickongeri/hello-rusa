<template>
  <q-layout view="lhh LpR lff">
    <q-header class="header-bg text-grey-9">
      <div
        class="row page-header items-center"
        style="height: 10vh; max-width: 1140px; margin: auto"
      >
        <router-link to="/">
          <div
            class="tabs-desktop q-my-md"
            style="font-weight: 700; min-width: 250px"
          >
            <q-img
              src="~src/assets/logo.svg"
              alt="Menopause app graphic"
              class="q-mb-md"
              style="max-width: 200px"
            />
          </div>
        </router-link>

        <div
          class="text-primary tabs-mobile q-ml-md text-h5"
          style="font-weight: 700"
        >
          <q-img
            src="~/src/assets/logo.svg"
            alt="Menopause app graphic"
            class="q-mb-md"
            style="max-width: 150px"
          />
        </div>
        <q-space />
        <div class="tabs-desktop">
          <q-tabs no-caps align="left">
            <q-route-tab to="/" label="Home" />
            <q-route-tab to="/page3" label="Download" />
            <q-route-tab to="/press" label="Press" />
            <q-route-tab to="/contact" label="Contact" />
          </q-tabs>
        </div>
        <div class="tabs-mobile q-mr-sm">
          <q-btn flat round color="primary" icon="mdi-menu" />
        </div>
      </div>
    </q-header>
    <q-footer>
      <div class="bg-grey-10" style="max-width: 100vw; height: 50vh">
        <div
          class="q-mx-auto row q-pa-md"
          style="min-height: 50vh; max-width: 1140px"
        >
          <div class="col-12 text-grey-1 col-md-6 flex flex-center">
            <div class="q-pr-md" style="width: 100%">
              <router-link to="/">
                <div class="text-h3 q-my-md" style="font-weight: 700">
                  <q-img
                    src="~/src/assets/whitelogo.svg"
                    alt="Menopause app graphic"
                    class="q-mb-md"
                    style="max-width: 150px"
                  />
                </div>
              </router-link>

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
      <!-- <q-toolbar>
        <q-toolbar-title>Footer</q-toolbar-title>
      </q-toolbar> -->
    </q-footer>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-page-sticky position="bottom-right" :offset="[18, 18]">
      <q-btn fab icon="keyboard_arrow_up" color="grey-10" />
    </q-page-sticky>
  </q-layout>
</template>

<script setup>
import { ref } from "vue";
import EssentialLink from "components/EssentialLink.vue";

const onDelayedClick = (e, go) => {
  e.preventDefault(); // mandatory; we choose when we navigate

  // console.log('triggering navigation in 2s')
  setTimeout(() => {
    // console.log('navigating as promised 2s ago')
    go();
  }, 2000);
};

const linksList = [
  {
    title: "Docs",
    caption: "quasar.dev",
    icon: "school",
    link: "https://quasar.dev",
  },
  {
    title: "Github",
    caption: "github.com/quasarframework",
    icon: "code",
    link: "https://github.com/quasarframework",
  },
  {
    title: "Discord Chat Channel",
    caption: "chat.quasar.dev",
    icon: "chat",
    link: "https://chat.quasar.dev",
  },
  {
    title: "Forum",
    caption: "forum.quasar.dev",
    icon: "record_voice_over",
    link: "https://forum.quasar.dev",
  },
  {
    title: "Twitter",
    caption: "@quasarframework",
    icon: "rss_feed",
    link: "https://twitter.quasar.dev",
  },
  {
    title: "Facebook",
    caption: "@QuasarFramework",
    icon: "public",
    link: "https://facebook.quasar.dev",
  },
  {
    title: "Quasar Awesome",
    caption: "Community Quasar projects",
    icon: "favorite",
    link: "https://awesome.quasar.dev",
  },
];

const leftDrawerOpen = ref(false);

function toggleLeftDrawer() {
  leftDrawerOpen.value = !leftDrawerOpen.value;
}
</script>

<style scoped>
.header-bg {
  background-color: #fbd2b4;
}
</style>
