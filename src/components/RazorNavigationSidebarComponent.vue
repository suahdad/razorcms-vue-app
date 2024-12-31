<script>
export default {
  name: "RazorNavigationSidebarComponent"
}
</script>

<template>
  <aside class="fixed bg-main h-dvh w-60">
    <nav>
      <header>
        <a href="#">BRAND</a>
      </header>
      <main>
      <ul>
          <li><a href="#">Dashboard</a></li>
          <li><a href="#">User Management</a></li>
          <li><a href="#">Documents</a></li>
          <li><a href="#">Statistics</a></li>
          <li><a href="#">Settings</a></li>
        </ul>
      </main>
      <footer class="absolute bottom-0 w-full">
        <a href="#" class="bg-sub">Logout</a>
      </footer>
    </nav>
  </aside>
</template>

<style scoped>

</style>