<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";

import AppAboutMe from "./components/AppAboutMe.vue";
import AppWhyWorkWithMe from "./components/AppWhyWorkWithMe.vue";
import AppViewAllWork from "./components/AppViewAllWork.vue";
import AppRecentWork from "./components/AppRecentWork.vue";
import AppPhotoCards from "./components/AppPhotoCards.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppAboutMe,
    AppFooter,
    AppWhyWorkWithMe,
    AppRecentWork,
    AppPhotoCards,
    AppViewAllWork,
  },
};
</script>

<template>
  <AppHeader />
  <AppAboutMe />
  <AppFooter />
  <AppWhyWorkWithMe />
  <AppRecentWork />
  <AppPhotoCards />
  <AppViewAllWork />
</template>

<style></style>
