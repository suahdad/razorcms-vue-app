<template>
  <header class="flex flex-col" role="banner">
    <div
        class="flex flex-wrap gap-5 justify-between px-6 py-5 w-full bg-white max-md:px-5 max-md:max-w-full"
    >
      <div class="flex gap-10 my-auto text-base">
        <h1 class="grow my-auto text-slate-400">Dashboard overview</h1>
        <form
            @submit.prevent="handleSearch"
            class="flex gap-2 px-4 py-3 rounded border border-solid border-slate-200 text-slate-300"
            role="search"
        >
          <label for="searchInput" class="sr-only">Search all</label>
          <img
              loading="lazy"
              src="https://cdn.builder.io/api/v1/image/assets/TEMP/a4379a63a653b91c1b3c89bb302bda25e155007856da5cf894d4b52ac6c4e233?placeholderIfAbsent=true&apiKey=b39d096ada144b56aa99e6a1c58c5780"
              class="object-contain shrink-0 self-start aspect-square fill-slate-300 w-[17px]"
              alt=""
          />
          <input
              type="search"
              id="searchInput"
              class="basis-auto bg-transparent border-none outline-none"
              placeholder="Search all..."
              v-model="searchQuery"
          />
        </form>
      </div>
      <div class="flex gap-10 items-center">
        <a
            href="#help"
            class="self-stretch my-auto text-xs text-slate-600 hover:underline focus:outline-none focus:ring-2 focus:ring-violet-700"
        >
          Help guides
        </a>
        <button
            class="flex gap-1 self-stretch my-auto text-xs whitespace-nowrap text-slate-600 hover:text-slate-800 focus:outline-none focus:ring-2 focus:ring-violet-700"
            @click="openInbox"
        >
          <span class="grow my-auto">Inbox</span>
          <div class="flex shrink-0 h-5 w-[23px]"></div>
        </button>
        <div class="flex gap-5 self-stretch">
          <button
              class="p-2 my-auto text-xs bg-violet-700 rounded text-slate-200 hover:bg-violet-800 focus:outline-none focus:ring-2 focus:ring-violet-700 focus:ring-offset-2"
              @click="downloadClient"
          >
            Download client
          </button>
          <div
              class="flex relative flex-col items-end px-2.5 pt-8 pb-px aspect-square w-[45px]"
              role="status"
              aria-label="User status indicator"
          >
            <img
                loading="lazy"
                src="https://cdn.builder.io/api/v1/image/assets/TEMP/1559f66e2e32bcb506d294498c3fc61b1e3a4960941c365634d005cde92815bf?placeholderIfAbsent=true&apiKey=b39d096ada144b56aa99e6a1c58c5780"
                class="object-cover absolute inset-0 size-full"
                alt="User profile"
            />
            <div
                class="flex relative shrink-0 w-full h-3 bg-green-400 rounded-full border border-white border-solid fill-green-400 stroke-[1px]"
            ></div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'RazorDashboardHeaderComponent',
  data() {
    return {
      searchQuery: ''
    }
  },
  methods: {
    handleSearch() {
      // Implement search functionality
    },
    openInbox() {
      // Implement inbox functionality
    },
    downloadClient() {
      // Implement download functionality
    }
  }
}
</script>

<style scoped>

</style>