<template>
  <div class="dark:bg-gray-900 dark:text-white">
    <nav
      class="flex justify-between items-center py-2 px-5 mb-5 bg-neutral-300 dark:bg-neutral-800"
    >
      <h1>Nuxt Blogs Project</h1>
      <p class="p-4 pb-2">
        <select
          v-model="$colorMode.preference"
          class="border w-24 h-8 dark:bg-gray-900 dark:text-white dark:border-gray-700"
        >
          <option value="light">Light</option>
          <option value="dark">Dark</option>
        </select>
      </p>
    </nav>
    <slot />
    <footer
      class="py-10 bg-neutral-400 dark:bg-neutral-800 px-5 mt-5 flex justify-center"
    >
      <span class="dark:text-gray-300">Created by Ivan Correa</span>
    </footer>
  </div>
</template>
