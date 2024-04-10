<template>
  <div
    class="quotation-marks-container skewed-container"
    :style="{ backgroundImage: `url(${backgroundImage})` }"
  >
    <div class="quotation-mark">
      <img src="/quotes-1.png" alt="Quotation Mark" />
    </div>
    <blockquote class="quotation">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod
        tempor incididunt ut labore et dolore magna aliqua.
      </p>
    </blockquote>
    <div class="circles">
      <div class="circle filled"></div>
      <!-- Filled circle -->
      <div class="circle"></div>
      <!-- Empty circle -->
    </div>
    <div class="global-brand">
      <!--  -->
      <p>Trusted by Global Brands</p>
    </div>
    <div class="vector-object">
      <!-- PNG images  -->
      <img
        src="/Vector_Smart_Object-1.png"
        alt="Image 1"
        style="margin-right: 10px"
      />
      <img
        src="/Vector_Smart_Object-2.png"
        alt="Image 2"
        style="margin-right: 10px"
      />
      <img
        src="/Vector_Smart_Object-3.png"
        alt="Image 3"
        style="margin-right: 10px"
      />
      <img
        src="/Vector_Smart_Object.png"
        alt="Image 4"
        style="margin-right: 10px"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "AppQuotationMarks",
  data() {
    return {
      backgroundImage: "/blog3-featured.jpg",
    };
  },
};
</script>

<style scoped>
.quotation-marks-container {
  text-align: center;
  padding: 100px;
  position: relative;
  background-size: cover;
  background-position: center;
  height: 500px;
}

.quotation-mark img {
  width: 50px;
}

.quotation,
.circle,
.circle.filled,
.global-brand {
  color: #fff;
}

.quotation {
  font-size: 20px;
}

.circle,
.circle.filled {
  display: inline-block;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  margin: 0 10px;
  border: 2px solid #fff; /* Empty circle */
  margin-bottom: -80px;
}

.circle.filled {
  background-color: #fff; /* Filled circle */
}

.global-brand {
  margin-top: 20px;
  font-size: 20px;
}

.vector-object {
  display: flex;
  justify-content: center;
}

.skewed-container {
  clip-path: polygon(
    0 0,
    100% 0,
    100% calc(100% - 5vw),
    0 100%
  ); /* clip-path inclination down */
}
.vector-object {
  display: flex;
  justify-content: center;

  margin-top: 100px;
}
</style>
