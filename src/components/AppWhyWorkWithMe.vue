<template>
  <!-- Sezione "Why Work With Me" -->
  <section class="why-work-section" style="background-color: #191c23">
    <h2>Why Work With Me</h2>
    <h3>Web Branding UX UI</h3>
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
    <!-- Icone Font Awesome -->
    <div class="icon-container">
      <!-- Web design -->
      <i class="fab fa-gitlab"></i>
      <!-- Web Design Icon -->
      <i class="fas fa-shield-alt"></i>
      <!-- diamnte -->
      <i class="fa-brands fa-sketch"></i>
      <!-- UX/UI Icon -->
    </div>
  </section>
</template>

<script>
export default {
  name: "AppWhyWorkWithMe",
};
</script>

<style scoped>
.why-work-section {
  color: #f2f2f2;
  height: 400px;
  padding: 20px;
  text-align: center;
  max-width: 100%;
  margin: 0 auto;
}

.icon-container {
  margin-top: 20px;
  display: flex;
  justify-content: center;
}

.icon-container i {
  font-size: 40px;
  margin: 0 20px;
}
i {
  color: #7a88ab;
}
</style>
