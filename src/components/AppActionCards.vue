<template>
  <div
    :style="{ backgroundColor: backgroundColor }"
    class="action-cards-container"
  >
    <div class="action-card" v-for="(card, index) in actionCards" :key="index">
      <div class="image-container">
        <img :src="card.imageSrc" :alt="card.alt" class="image" />
      </div>
      <div class="overlay">
        <span class="overlay-text">{{ card.title }}</span>
      </div>
      <h2>{{ card.title }}</h2>
      <p>{{ card.description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppActionCards",
  data() {
    return {
      backgroundColor: "#1D2028",
      actionCards: [
        {
          imageSrc: "/blog1-featured.jpg",
          alt: "Image 1",
          title: "Live The design Process",
          description:
            "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Iure modi maxime libero maiores debitis, velit, quos temporibus aliquid dolor id quis nesciunt quasi tempore veritatis, nam officiis! Ipsa, neque corporis!",
        },
        {
          imageSrc: "/blog2-featured.jpg",
          alt: "Image 2",
          title: "What next of the app store?",
          description:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ratione inventore veniam beatae, minima incidunt adipisci quam! Temporibus placeat inventore, ducimus optio cupiditate eaque! Optio voluptatibus voluptate, facilis corporis temporibus officia.",
        },
        {
          imageSrc: "/blog3-featured.jpg",
          alt: "Image 3",
          title: "The Humble Wooden Desk",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis alias, accusamus non tenetur, voluptate optio ex totam ratione laboriosam eius culpa, labore recusandae quae itaque illum natus neque veniam nam!",
        },
      ],
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
  position: relative;
}

.action-card img {
  max-width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(255, 0, 0, 0.5); /* trasparen of 50% */
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

.action-card:hover .overlay {
  opacity: 1; /* showvl'overlay quando il mouse on the card */
}

h2 {
  margin-top: 20px;
  font-size: 28px;
  color: #ff0000;
}

p {
  margin-top: 10px;
  font-size: 18px;
}
.image-container {
  width: 100%;
  height: 200px;
  overflow: hidden;
}

.image {
  width: 100%; /* Assicura che l'immagine si adatti completamente al suo contenitore */
  height: auto; /* Lascia che l'altezza sia proporzionale alla larghezza per evitare distorsioni */
}
</style>
