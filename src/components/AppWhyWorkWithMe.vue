<template>
  <!-- Sezione "Why Work With Me" -->
  <section class="why-work-section">
    <div class="skewed-container top">
      <h2>Why Work With Me</h2>
      <h3>Web Branding UX UI</h3>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vehicula
        dolor non justo efficitur hendrerit. Nam ac eros in tellus dapibus
        placerat. Nulla facilisi. Donec congue magna id justo tincidunt rhoncus.
        Suspendisse vel ultricies enim, ac hendrerit tortor. Vestibulum
        vestibulum orci non ipsum semper, ac ultricies leo luctus. Vestibulum
        aliquet semper leo, non condimentum nisi volutpat in. Nam venenatis mi
        et elit rhoncus, nec sodales sapien aliquet. Sed fringilla mi et ex
        fermentum ultricies. Morbi in sapien luctus, bibendum lorem eu, lacinia
        magna. Integer et dolor id libero sollicitudin pulvinar.
      </p>
      <!-- Icone Font Awesome con cerchi di caricamento -->
      <div class="icon-container">
        <!-- Web design -->
        <div class="icon-wrapper">
          <i class="fab fa-gitlab"></i>
          <svg class="loading-circle" style="position: absolute">
            <circle
              class="circle"
              cx="50%"
              cy="50%"
              r="40"
              :style="{
                strokeDasharray: '251.2',
                strokeDashoffset: calculateDashOffset(dashoffsetData.web),
              }"
            ></circle>
          </svg>
        </div>
        <!-- Web Design Icon -->
        <div class="icon-wrapper">
          <i class="fas fa-shield-alt"></i>
          <svg class="loading-circle" style="position: absolute">
            <circle
              class="circle"
              cx="50%"
              cy="50%"
              r="40"
              :style="{
                strokeDasharray: '251.2',
                strokeDashoffset: calculateDashOffset(dashoffsetData.design),
              }"
            ></circle>
          </svg>
        </div>
        <!-- UX/UI Icon -->
        <div class="icon-wrapper">
          <i class="fa-brands fa-sketch"></i>
          <svg class="loading-circle" style="position: absolute">
            <circle
              class="circle"
              cx="50%"
              cy="50%"
              r="40"
              :style="{
                strokeDasharray: '251.2',
                strokeDashoffset: calculateDashOffset(dashoffsetData.ux),
              }"
            ></circle>
          </svg>
        </div>
      </div>
    </div>
    <div class="skewed-container bottom"></div>
  </section>
</template>

<script>
export default {
  name: "AppWhyWorkWithMe",
  data() {
    return {
      dashoffsetData: {
        web: 80, // Percentuale di caricamento per l'icona Web Design
        design: 70, // Percentuale di caricamento per l'icona Design
        ux: 90, // Percentuale di caricamento per l'icona UX/UI
      },
    };
  },
  methods: {
    calculateDashOffset(percent) {
      const circumference = 251.2; // Circonferenza del cerchio (2 * pi * r)
      const percentage = percent / 100;
      return circumference * (1 - percentage);
    },
  },
};
</script>

<style scoped>
.why-work-section {
  color: #f2f2f2;
  text-align: center;
  max-width: 100%;
  margin-top: -80px;
  margin-bottom: -80px;
}

.skewed-container {
  background-color: #191c23;
  padding: 50px 0;
}

.skewed-container.top {
  clip-path: polygon(0 0, 100% 5vw, 100% 100%, 0 100%);
}

.skewed-container.bottom {
  clip-path: polygon(0 0, 100% 0, 100% calc(100% - 5vw), 0 100%);
}

.icon-container {
  margin-top: 20px;
  display: flex;
  justify-content: center;
}

.icon-wrapper {
  position: relative;
  margin: 0 auto;
}

.icon-wrapper i {
  font-size: 50px;
  color: #7a88ab;
}

.loading-circle {
  width: 80px;
  height: 80px;
  /* margin-right: 50px; */
  margin-left: -69px;
  /* display: flex; */
  align-content: flex-start;
  flex-wrap: wrap;
  flex-direction: row-reverse;
  justify-content: space-evenly;
  align-items: flex-end;
}

.circle {
  fill: none;
  stroke: red; /* Colore del tratto */
  stroke-width: 4; /* Spessore del tratto */
  stroke-linecap: round; /* Estremità del tratto rotonda */
}
</style>
