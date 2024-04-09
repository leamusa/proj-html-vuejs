<template>
  <div class="lets-work-together-container">
    <h2 class="title">Let's Work Together</h2>
    <h3 class="subtitle">Get in Touch</h3>
    <hr />
    <form @submit.prevent="submitForm">
      <div class="form-group">
        <input type="text" v-model="name" placeholder="Name" required />
      </div>
      <div class="form-group">
        <input type="email" v-model="email" placeholder="Email" required />
      </div>
      <div class="form-group">
        <input type="tel" v-model="phone" placeholder="Phone" required />
      </div>
      <button type="submit">Let's Talk</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "AppLetsWorkTogether",
  data() {
    return {
      name: "",
      email: "",
      phone: "",
    };
  },
};
</script>

<style scoped>
.lets-work-together-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 50px;
  background-color: #c7cbd4;
}

.title,
.subtitle {
  color: #000;
}

.lets-work-together-container hr {
  margin: 20px auto;
  width: 50%;
  border-color: #000;
}

.form-group {
  margin-bottom: 20px;
}

.form-group input {
  width: 300px;
  padding: 15px 20px;
  font-size: 16px;
  border: none;
  background-color: #fff;
  color: #191c23;
}

button {
  padding: 15px 40px;
  font-size: 16px;
  background-color: #ff0000;
  color: #fff;
  border: none;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

button:hover {
  background-color: #151414;
}
</style>
