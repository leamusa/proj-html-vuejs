<template>
  <div class="recent-work-container">
    <h2>Recent Work</h2>
    <ul>
      <li v-for="(item, index) in recentWorkItems" :key="index">
        {{ item.title }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "AppRecentWork",
  data() {
    return {
      recentWorkItems: [
        { title: "Web" },
        { title: "Branding" },
        { title: "UI, UX" },
      ],
    };
  },
};
</script>

<style>
.recent-work-container {
  text-align: center;
  background-color: #96c577;
  padding: 20px;
}

/* Element of list */
.recent-work-container ul {
  list-style-type: none;
  padding: 0;
  display: flex;
  justify-content: space-evenly;
}
</style>
