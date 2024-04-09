<script>
import AppHeader from "./components/AppHeader.vue";

import AppAboutMe from "./components/AppAboutMe.vue";
import AppWhyWorkWithMe from "./components/AppWhyWorkWithMe.vue";
import AppViewAllWork from "./components/AppViewAllWork.vue";
import AppRecentWork from "./components/AppRecentWork.vue";
import AppPhotoCards from "./components/AppPhotoCards.vue";
import AppQuotationMarks from "./components/AppQuotationMarks.vue";
import AppExpertDesignAdvice from "./components/AppExpertDesignAdvice.vue";
import AppActionCards from "./components/AppActionCards.vue";
import AppLetsWorkTogether from "./components/AppLetsWorkTogether.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppAboutMe,
    AppWhyWorkWithMe,
    AppRecentWork,
    AppPhotoCards,
    AppViewAllWork,
    AppQuotationMarks,
    AppExpertDesignAdvice,
    AppActionCards,
    AppLetsWorkTogether,
    AppFooter,
  },
};
</script>

<template>
  <AppHeader />
  <AppAboutMe />

  <AppWhyWorkWithMe />
  <AppRecentWork />
  <AppPhotoCards />
  <AppViewAllWork />
  <AppQuotationMarks />
  <AppExpertDesignAdvice />
  <AppActionCards />
  <AppLetsWorkTogether />
  <AppFooter />
</template>

<style></style>
