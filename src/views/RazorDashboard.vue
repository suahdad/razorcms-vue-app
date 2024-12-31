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
<razor-navigation-sidebar-component></razor-navigation-sidebar-component>
<main>
  <header>
    <razor-search-component></razor-search-component>
  </header>
  <razor-table-component></razor-table-component>
  <footer></footer>
</main>

</template>

<style scoped>

</style>