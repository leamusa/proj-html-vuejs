<template>
  <div class="view-all-work">
    <h2 @click="toggleContent">View all the work</h2>
    <div v-if="showContent" class="additional-content"></div>
  </div>
</template>

<script>
export default {
  name: "AppViewAllWork",
  data() {
    return {
      showContent: false,
    };
  },
  methods: {
    toggleContent() {
      this.showContent = !this.showContent;
    },
  },
};
</script>

<style scoped>
.view-all-work {
  text-align: center;
  background-color: #f9225b;
  max-width: 100%;
  height: 100px;
  padding: 5px;
  color: #ffff;
}

.view-all-work h2 {
  cursor: pointer; /* Imposta il cursore a forma di mano quando si passa sopra al titolo */
}
</style>
