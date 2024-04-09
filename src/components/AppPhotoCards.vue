<template>
  <div class="photo-cards-container">
    <div class="photo-grid">
      <template v-for="(photo, index) in photos" :key="index">
        <div class="photo-card">
          <img :src="photo.url" :alt="photo.alt" class="photo" />
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

<style>
.photo-cards-container {
  text-align: center;
}

.photo-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding: 0;
}

.photo-card {
  width: 30%;
  margin-bottom: -10px;
}

.photo {
  width: 100%;
  height: auto;
}
</style>
