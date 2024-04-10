<template>
  <!-- Sezione "About Me" -->
  <section class="about-section skewed-container bottom">
    <h2>About Me</h2>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vehicula
      dolor non justo efficitur hendrerit. Nam ac eros in tellus dapibus
      placerat. Nulla facilisi. Donec congue magna id justo tincidunt rhoncus.
      Suspendisse vel ultricies enim, ac hendrerit tortor. Vestibulum vestibulum
      orci non ipsum semper, ac ultricies leo luctus. Vestibulum aliquet semper
      leo, non condimentum nisi volutpat in. Nam venenatis mi et elit rhoncus,
      nec sodales sapien aliquet. Sed fringilla mi et ex fermentum ultricies.
      Morbi in sapien luctus, bibendum lorem eu, lacinia magna. Integer et dolor
      id libero sollicitudin pulvinar.
    </p>
  </section>
</template>

<script>
export default {
  name: "AppAboutMe",
};
</script>

<style scoped>
.about-section {
  background-color: #1d2028;
  padding: 20px;
  text-align: center;
  color: #fff;
  height: 400px;
}

.skewed-container {
  clip-path: polygon(0 calc(100% - 5vw), 100% 100%, 100% 0, 0 0);
}
</style>
