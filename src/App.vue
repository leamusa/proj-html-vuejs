<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";

import AppAboutMe from "./components/AppAboutMe.vue";
import AppWhyWorkWithMe from "./components/AppWhyWorkWithMe.vue";
export default {
  name: "App",
  components: {
    AppHeader,
    AppAboutMe,
    AppFooter,
    AppWhyWorkWithMe,
  },
};
</script>

<template>
  <AppHeader />
  <AppAboutMe />
  <AppFooter />
  <AppWhyWorkWithMe />
</template>

<style></style>
