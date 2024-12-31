<script>
import RazorNavigationSidebarComponent from "@/components/RazorNavigationSidebarComponent.vue";
import RazorTableComponent from "@/components/RazorTableComponent.vue";
import RazorSearchComponent from "@/components/RazorSearchComponent.vue";

export default {
  name: "RazorDashboard",
  components: {RazorSearchComponent, RazorTableComponent, RazorNavigationSidebarComponent},
}
</script>

<template>
<header>
  <razor-search-component></razor-search-component>
</header>
<aside class="left-section">
  <razor-navigation-sidebar-component></razor-navigation-sidebar-component>
</aside>
<aside class="right-section"></aside>
<main>
  <razor-table-component></razor-table-component>
</main>
<footer></footer>
</template>

<style scoped>

</style>