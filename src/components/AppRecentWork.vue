<template>
  <div class="recent-work-container">
    <h2>Recent Work</h2>
    <ul>
      <li><span class="bullet"></span> Web</li>
      <li><span class="bullet"></span> Branding</li>
      <li><span class="bullet"></span> UI, UX</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "AppRecentWork",
};
</script>

<style>
.recent-work-container {
  text-align: center;
  background-color: #96c577;
  padding: 20px;
}
.bullet,
.recent-work-container ul {
  list-style-type: none;
  padding: 0;
  display: flex;
  justify-content: center;

  color: #fff;
}

.recent-work-container ul li {
  position: relative;
}

.bullet {
  display: inline-block;
  width: 5px;
  height: 5px;
  background-color: #fff;
  border-radius: 50%;
  margin-right: 10px;
  margin-left: 10px;
}
h2 {
  margin-top: 50px;
  color: #fff;
}
</style>
