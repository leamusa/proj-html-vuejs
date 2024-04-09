<template>
  <div
    class="quotation-marks-container"
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
  background: url(/blog3-featured.jpg) center/cover;
  text-align: center;
  padding: 50px;
}

.quotation-mark img {
  width: 50px; /* Set the width of the quotation mark image */
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
}

.circle.filled {
  background-color: #fff; /* Filled circle */
}

.global-brand {
  margin-top: 20px;
  font-size: 20px;
}
</style>
