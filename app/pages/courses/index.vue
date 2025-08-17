<template>
  <!-- TODO: fill courses -->
  <UiAuroraBackground>
    <Motion
      as="div"
      :initial="{ opacity: 0, y: 40, filter: 'blur(10px)' }"
      :while-in-view="{
        opacity: 1,
        y: 0,
        filter: 'blur(0px)',
      }"
      :transition="{
        delay: 0.3,
        duration: 0.8,
        ease: 'easeInOut',
      }"
      class="relative flex flex-col items-center justify-center gap-4 px-4"
    >
      <div class="text-center text-3xl font-bold md:text-7xl dark:text-white">
        Courses page is building
      </div>
      <div
        class="py-4 text-base font-extralight md:text-4xl dark:text-neutral-200"
      >
        Check it on
        <NuxtLink
          class="text-blue-600 dark:text-blue-400 cursor-pointer hover:underline"
          to="https://github.com/13rtk"
          target="_blank"
        >
          GitHub
        </NuxtLink>
        /
        <NuxtLink
          class="text-pink-600 dark:text-pink-400 cursor-pointer hover:underline"
          to="https://github.com/13rtk"
          target="_blank"
        >
          Bilibili
        </NuxtLink>
      </div>
      <button
        class="w-fit rounded-full bg-black px-4 py-2 text-white dark:bg-white dark:text-black cursor-pointer hover:opacity-80 transition-opacity"
        @click="() => $router.push('/')"
      >
        Back Home
      </button>
    </Motion>
  </UiAuroraBackground>
</template>

<script setup lang="ts">
import { Motion } from 'motion-v';
</script>
