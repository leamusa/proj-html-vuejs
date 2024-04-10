<template>
  <div class="photo-cards-container">
    <div class="photo-grid">
      <template v-for="photo in photos" :key="index">
        <div class="photo-card">
          <img :src="photo.url" :alt="photo.alt" class="photo" />
          <div class="overlay">
            <span class="overlay-text">Flat Picture Frame</span>
          </div>
        </div>
      </template>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppPhotoCards",
  data() {
    return {
      photos: [
        { url: "/portfolio1_featured_item-400x320.jpg", alt: "Photo 1" },
        { url: "/portfolio2_featured_item-400x320.jpg", alt: "Photo 2" },
        { url: "/portfolio3_featured_item-400x320.jpg", alt: "Photo 3" },
        { url: "/portfolio4_featured_item-400x320.jpg", alt: "Photo 4" },
        { url: "/portfolio5_featured_item-400x320.jpg", alt: "Photo 5" },
        { url: "/portfolio6_featured_item-400x320.jpg", alt: "Photo 6" },
      ],
    };
  },
};
</script>

<style scoped>
.photo-cards-container {
  text-align: center;
}

.photo-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.photo-card {
  width: 30%;
  margin-bottom: -10px;
  position: relative; /* position relative for'overlay(absolute) */
}

.photo {
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(
    255,
    0,
    0,
    0.5
  ); /* Imposta il colore rosso con una trasparenza del 50% */
  display: flex;
  justify-content: center;
  align-items: center;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.overlay-text {
  color: white;
  font-size: 24px;
}

.photo-card:hover .overlay {
  opacity: 1; /*shwo overlay on the card*/
}
</style>
