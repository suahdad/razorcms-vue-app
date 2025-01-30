<script>
import RazorNavigationSidebarComponent from "@/components/RazorNavigationSidebarComponent.vue";
import RazorTableComponent from "@/components/RazorTableComponent.vue";
import RazorDashboardHeaderComponent from "@/components/RazorDashboardHeaderComponent.vue";

export default {
  name: "RazorDashboard",
  components: {RazorDashboardHeaderComponent, RazorTableComponent, RazorNavigationSidebarComponent},
}
</script>

<template>
<razor-navigation-sidebar-component></razor-navigation-sidebar-component>
<main>
  <header>
    <razor-dashboard-header-component></razor-dashboard-header-component>
  </header>
  <razor-table-component></razor-table-component>
  <footer></footer>
</main>

</template>

<style scoped>
main {
  position: fixed;
  left: var(--sidebar-width);
  width: calc(100% - var(--sidebar-width));
}

main>header {
  line-height: var(--main-header-height);
  max-height: var(--main-header-height);
  overflow: hidden;
}

</style>