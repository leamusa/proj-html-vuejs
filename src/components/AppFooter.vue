<template>
  <footer class="footer-container">
    <div class="logo-container">
      <img src="/avada-footer-logo.png" alt="Logo" />
    </div>
    <div class="copyright-container">
      <p>
        © Copywrite 2012 - 2020 | Avada theme fusion | All rights reserved |
        Powered by Wordpress
      </p>
    </div>
    <div class="social-icons-container">
      <div class="social-icon">
        <i class="fab fa-facebook-f"></i>

        <i class="fab fa-twitter"></i>

        <i class="fab fa-instagram"></i>

        <i class="fab fa-youtube"></i>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
};
</script>

<style scoped>
.footer-container {
  background-color: #1d2028;
  color: #fff;
  padding: 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  flex-direction: column;
}

.logo-container img {
  width: 100px;
}

.copyright-container {
  font-size: 12px;
}

.social-icons-container {
  display: flex;
}

.social-icon {
  margin-right: 10px;
}

.social-icon i {
  font-size: 24px;
}
</style>
