<template>
  <header
    class="header"
    :style="{ backgroundImage: `url(${backgroundImage})` }"
  >
    <!-- Container for the header content -->
    <div class="header-content">
      <!-- Logo of the application -->
      <div class="logo">
        <!-- Dynamic image source bound to the "logoSrc" data property -->
        <img :src="logoSrc" alt="Logo" />
      </div>
      <!-- Container for the menu items -->
      <div class="menu">
        <!-- plus button -->
        <button class="plus-button" @click="togglePlus">
          <!-- Plus sign symbol -->
          <span>+</span>
        </button>
        <!-- Button to toggle  -->
        <button class="navbar-toggler" @click="toggleOffcanvas">
          <!--  hamburger icon -->
          <span class="line"></span>
          <span class="line"></span>
          <span class="line"></span>
        </button>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  // Component name
  name: "AppHeader",
  // Data properties
  data() {
    return {
      // logo
      logoSrc: "/avada-freelance-logo.png",
      // background image
      backgroundImage: "/freelancer_thumbnail.jpg",
    };
  },
  // Methods
};
</script>

<style scoped>
.navbar-toggler {
  background-color: transparent;
  border: none;
  cursor: pointer;
  padding: 5px;
}

.line {
  display: block;
  width: 25px;
  height: 3px;
  background-color: white;
  margin-bottom: 5px;
}

/* Stili per l'header */
.header {
  padding: 10px 20px;
  background-color: #333;
  background-size: cover;
  background-position: center;
  max-width: 100%;
  height: 700px;
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  width: 100px;
}

.plus-button {
  background-color: transparent;
  border: none;
  cursor: pointer;
  font-size: 18px;
  color: white;
}

.plus-button:hover {
  background-color: #0056b3;
}
</style>
