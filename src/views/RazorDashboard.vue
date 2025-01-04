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
  <header class="px-5 flex gap-9">
    <h3 class="inline">Dashboard Overview</h3>
    <razor-search-component></razor-search-component>
    <div id="action-bar" class="ml-auto flex gap-9">
      <a class="" href="#">Help Guide</a>
      <a class="" href="">Inbox</a>
      <button class="">Download Client</button>
      <a class="" href="#">ClientPhoto</a>
    </div>
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