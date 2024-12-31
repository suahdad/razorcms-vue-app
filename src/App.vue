<template>
<RazorDashboard></RazorDashboard>
</template>

<script>
import RazorDashboard from "@/views/RazorDashboard.vue";
import "./assets/index.css";

export default {
  name: 'App',
  components: {
    RazorDashboard
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
