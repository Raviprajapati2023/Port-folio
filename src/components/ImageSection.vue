<template>
  <div class="mt-16 sm:mt-20 overflow-hidden">
    <div
      class="-my-4 flex flex-row justify-center gap-5 overflow-hidden py-4 sm:gap-8"
    >
      <div
        class="relative aspect-[9/10] w-44 overflow-hidden rounded-xl bg-zinc-100 dark:bg-zinc-800 sm:w-72 sm:rounded-2xl rotate-1"
        v-for="i in images"
        :key="i.img"
      >
        <img
          loading="lazy"
          width="3744"
          height="5616"
          decoding="async"
          data-nimg="1"
          class="absolute inset-0 h-full w-full"
          style="color: transparent"
          sizes="(min-width: 640px) 18rem, 11rem"
          :src="i.img"
        />
      </div>
    </div>
  </div>
</template>
<script setup>
const images = [
  {
    img: "",
  },
  {
    img: "",
  },
  {
    img: "",
  },
  {
    img: "",
  },
];
</script>
