<script>
export default {
  name: "RazorTableComponent"
}
</script>

<template>
  <div class="p-6 bg-white rounded-md shadow-[0_2px_4px_rgba(0,0,0,0.1)]">
    <div class="flex justify-between items-center mb-5">
      <div class="flex gap-2 items-center text-xl text-slate-600">
        <span>Order catalogue</span>
        <span class="px-1.5 py-1 text-xs text-white bg-teal-300 rounded">New items</span>
      </div>
      <div class="flex gap-4 items-center max-md:flex-wrap max-sm:flex-col">
        <div class="flex gap-2 items-center px-4 py-2.5 rounded border border-solid border-slate-200 text-slate-300 max-sm:w-full" tabindex="0">
          <span>Select column</span>
          <i class="ti ti-chevron-down"></i>
        </div>
        <div class="flex gap-2 items-center px-4 py-2.5 rounded border border-solid border-slate-200 text-slate-300 max-sm:w-full" tabindex="0">
          <i class="ti ti-search"></i>
          <span>Search list...</span>
        </div>
        <i class="ti ti-adjustments" tabindex="0"></i>
        <div class="px-4 py-2.5 text-white bg-violet-900 rounded cursor-pointer" tabindex="0">Add new</div>
      </div>
    </div>
    <table class="mt-5 w-full border-collapse max-sm:block max-sm:overflow-x-auto">
      <thead>
        <tr>
          <th class="p-3 font-medium text-left bg-slate-100 text-slate-600">#</th>
          <th class="p-3 font-medium text-left bg-slate-100 text-slate-600">Product</th>
          <th class="p-3 font-medium text-left bg-slate-100 text-slate-600">Serial-code</th>
          <th class="p-3 font-medium text-left bg-slate-100 text-slate-600">Stock</th>
          <th class="p-3 font-medium text-left bg-slate-100 text-slate-600">Category</th>
          <th class="p-3 font-medium text-left bg-slate-100 text-slate-600">Actions</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="px-3 py-4 border-b border-solid border-b-slate-200 text-slate-500">03</td>
          <td class="px-3 py-4 border-b border-solid border-b-slate-200 text-slate-500">Macbook pro 16</td>
          <td class="px-3 py-4 border-b border-solid border-b-slate-200 text-slate-500">#123-456ABC</td>
          <td class="px-3 py-4 border-b border-solid border-b-slate-200 text-slate-500">123</td>
          <td class="px-3 py-4 border-b border-solid border-b-slate-200 text-slate-500">Apple</td>
          <td class="flex gap-5 px-3 py-4 border-b border-solid border-b-slate-200 text-slate-500" tabindex="0">
            <span class="cursor-pointer text-slate-500">Edit</span>
            <span class="cursor-pointer text-slate-500">Delete</span>
          </td>
        </tr>
        <!-- Repeat for additional rows -->
      </tbody>
    </table>
    <div class="flex gap-4 justify-end items-center mt-5 text-sm text-slate-300">
      <i class="ti ti-chevron-left" tabindex="0"></i>
      <div class="flex gap-2 items-center">
        <span>1</span>
        <div class="w-6 h-6 text-white bg-pink-400 rounded-full cursor-pointer" tabindex="0">2</div>
        <span>3</span>
        <span>4</span>
        <span>. . . 10</span>
      </div>
      <i class="ti ti-chevron-right" tabindex="0"></i>
      <div class="flex gap-2 items-center px-3 py-2 rounded border border-solid border-slate-200 cursor-pointer" tabindex="0">
        <span>Display 10 items</span>
        <i class="ti ti-chevron-down"></i>
      </div>
    </div>
  </div>
</template>

<style scoped>
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
</style>