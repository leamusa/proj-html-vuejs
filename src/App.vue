<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";

import AppAboutMe from "./components/AppAboutMe.vue";
import AppWhyWorkWithMe from "./components/AppWhyWorkWithMe.vue";
import AppViewAllWork from "./components/AppViewAllWork.vue";
import AppRecentWork from "./components/AppRecentWork.vue";
import AppPhotoCards from "./components/AppPhotoCards.vue";
import AppQuotationMarks from "./components/AppQuotationMarks.vue";
import AppExpertDesignAdvice from "./components/AppExpertDesignAdvice.vue";

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
    AppQuotationMarks,
    AppExpertDesignAdvice,
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
  <AppQuotationMarks />
  <AppExpertDesignAdvice />
</template>

<style></style>
