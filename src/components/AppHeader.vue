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
        <!-- Plus button -->
        <button class="plus-button" @click="togglePlus">
          <!-- Plus sign symbol -->
          <span class="plus-symbol">+</span>
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
    <!-- Title "Avada Freelance" in white -->
    <h2 class="title-white">Avada Freelance</h2>
    <!-- Title "Art Director" in red, centered, and larger -->
    <h1 class="title-red">Art Director</h1>
    <!-- Title with transparency "If you want everything is going to change" -->
    <h3 class="transparent-title">If you want everything is going to change</h3>
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
      backgroundImage: "/banner_images.jpg",
    };
  },
  // Methods
};
</script>

<style scoped>
/* Styles for the header */
.header {
  padding: 10px 20px;
  background-color: #333;
  background-size: cover;
  background-position: center;
  max-width: 100%;
  height: 700px;
  position: relative;
}

.header-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1;
  padding: 20px;
  width: 100%;
}

.logo {
  width: 100px;
}

.menu {
  display: flex;
  align-items: start;
}

.menu button {
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

.plus-symbol {
  font-size: 24px;
  color: white;
}

.title-white {
  color: white;
  font-size: 24px;
  text-align: center;
  margin-top: 50px;
}

.title-red {
  color: #ff0000;
  font-size: 48px;
  text-align: center;
}

.transparent-title {
  color: white;
  font-size: 36px;
  opacity: 0.7;
  text-align: center;
}
</style>
