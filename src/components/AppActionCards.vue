<template>
  <div
    :style="{ backgroundColor: backgroundColor }"
    class="action-cards-container"
  >
    <div class="action-card">
      <img src="/blog1-featured.jpg" alt="Image 1" />
      <h2>Title 1</h2>
      <p>Subtitle 1</p>
    </div>
    <div class="action-card">
      <img src="/blog2-featured.jpg" alt="Image 2" />
      <h2>Title 2</h2>
      <p>Subtitle 2</p>
    </div>
    <div class="action-card">
      <img src="/blog3-featured.jpg" alt="Image 3" />
      <h2>Title 3</h2>
      <p>Subtitle 3</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppActionCards",
  data() {
    return {
      backgroundColor: "#1D2028",
    };
  },
};
</script>

<style scoped>
.action-cards-container {
  display: flex;
  justify-content: space-around;
}

.action-card {
  text-align: center;
  padding: 20px;
}

.action-card img {
  max-width: 100%;
  height: auto;
}

.action-card h2 {
  margin-top: 20px;
  font-size: 28px; /* Titolo più grande */
  color: #ff0000; /* Rosso */
}

.action-card p {
  margin-top: 10px;
  font-size: 18px;
}
</style>
