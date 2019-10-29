<template>
  <div>
    <h1>The User Page</h1>
    <hr />
    <router-view></router-view>
    <button @click="navigateToHome" class="btn btn-info">Go to Home</button>
  </div>
</template>

<script>
export default {
  methods: {
    navigateToHome() {
      this.$router.push({ name: "home" });
    }
  }
};
</script>