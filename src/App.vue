<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";

import AppAboutMe from "./components/AppAboutMe.vue";
export default {
  name: "App",
  components: {
    AppHeader,
    AppAboutMe,
    AppFooter,
  },
};
</script>

<template>
  <AppHeader />
  <AppAboutMe />
  <AppFooter />
</template>

<style></style>
