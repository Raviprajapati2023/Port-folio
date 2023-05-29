<template>
  <footer class="mt-32">
    <div class="sm:px-8">
      <div class="mx-auto max-w-7xl p-0 lg:px-8">
        <div
          class="border-t border-zinc-100 pb-16 pt-10 dark:border-zinc-700/40"
        >
          <div class="relative px-4 sm:px-8 lg:px-12">
            <div class="mx-auto max-w-2xl lg:max-w-5xl">
              <div
                class="flex flex-col items-center justify-between gap-6 sm:flex-row"
              >
                <div
                  class="flex flex-wrap justify-center gap-x-6 gap-y-1 text-sm font-medium text-zinc-800 dark:text-zinc-200"
                >
                  <div v-for="p in pages" :key="p.name">
                    <router-link
                      class="transition hover:text-teal-500 dark:hover:text-teal-400"
                      :to="p.link"
                      >{{ p.name }}</router-link
                    >
                  </div>
                </div>
                <p class="text-sm text-zinc-400 dark:text-zinc-500">
                  ©
                  <!-- -->2023<!-- -->
                  Spencer Sharp. All rights reserved.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>
<script setup>
const pages = [
  {
    link: "/about",
    name: "About",
  },
  {
    link: "/projects",
    name: "Projects",
  },
  {
    link: "/speaking",
    name: "Speaking",
  },
  {
    link: "/uses",
    name: "Uses",
  },
];
</script>
