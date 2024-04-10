<template>
  <div class="skewed-container bottom">
    <div class="expert-design-advice">
      <h2 class="title">Expert Design Advice</h2>
      <h3 class="subtitle">Trending Design News</h3>
      <hr class="line" />
    </div>
  </div>
</template>

<script>
export default {
  name: "AppExpertDesignAdvice",
};
</script>

<style scoped>
.skewed-container.bottom {
  clip-path: polygon(0 5vw, 100% 0, 100% 100%, 0 100%);
}

.expert-design-advice {
  background-color: #49629b;
  padding: 20px;
  text-align: center;
  color: #fff;
  margin-top: -80px;
}

.title {
  font-size: 24px;
  margin-bottom: 10px;
}

.subtitle {
  font-size: 18px;
  margin-bottom: 20px;
}

.line {
  width: 50%;
  margin: auto;
  border: 1px solid #fff;
}
</style>
