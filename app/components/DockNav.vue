<template>
  <UiDock class="mb-6">
    <!-- Home -->
    <UiDockIcon class="group flex flex-row items-center">
      <div class="tooltip tooltip-bottom">
        <div class="tooltip-content dark:bg-white">
          <div
            class="animate-bounce dark:text-orange-400 -rotate-10 text-2xl font-black text-blue-600"
          >
            Back Home
          </div>
        </div>
        <Icon
          icon="ic:baseline-home"
          class="text-blue-500 dark:text-blue-200 text-4xl opacity-70 group-hover:text-orange-500 transition-opacity"
          @click="() => $router.push('/')"
        />
      </div>
    </UiDockIcon>
    <UiDockSeparator />
    <!-- Blogs -->
    <UiDockIcon class="group flex flex-row items-center">
      <div class="tooltip tooltip-bottom">
        <div class="tooltip-content dark:bg-white">
          <div
            class="animate-bounce dark:text-orange-400 -rotate-10 text-2xl font-black text-blue-600"
          >
            Blogs
          </div>
        </div>
        <!-- TODO: Add link to blogs -->
        <Icon
          icon="ic:baseline-edit-note"
          class="text-blue-500 dark:text-blue-200 text-4xl opacity-70 group-hover:text-orange-500 transition-opacity"
          @click="() => toast.info({ title: 'Coming soon' })"
        />
      </div>
    </UiDockIcon>
    <UiDockSeparator />
    <!-- Courses -->
    <UiDockIcon class="group flex flex-row items-center">
      <div class="tooltip tooltip-bottom">
        <div class="tooltip-content dark:bg-white">
          <div
            class="animate-bounce dark:text-orange-400 -rotate-10 text-2xl font-black text-blue-600"
          >
            Courses
          </div>
        </div>
        <!-- TODO: Add link to courses -->
        <Icon
          icon="material-symbols:book-2"
          class="text-blue-500 dark:text-blue-200 text-4xl opacity-70 group-hover:text-orange-500 transition-opacity"
          @click="() => toast.info({ title: 'Coming soon' })"
        />
      </div>
    </UiDockIcon>
    <UiDockSeparator />
    <!-- Contact -->
    <UiDockIcon group flex flex-row items-center>
      <div class="tooltip tooltip-bottom">
        <div class="tooltip-content dark:bg-white">
          <div
            class="animate-bounce dark:text-orange-400 -rotate-10 text-2xl font-black text-green-600"
          >
            Contact
          </div>
        </div>
        <Icon
          icon="mdi:email"
          class="text-green-500 dark:text-green-200 text-4xl group-hover:text-orange-500 opacity-70 transition-opacity"
          @click="() => toast.info({ title: 'Coming soon' })"
        />
      </div>
    </UiDockIcon>
  </UiDock>
</template>

<script setup lang="ts">
import { Icon } from '@iconify/vue';

const toast = useToast();
</script>
