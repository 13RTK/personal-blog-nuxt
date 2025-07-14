<script setup lang="ts">
/** biome-ignore-all lint/correctness/noUnusedImports: false */
import { Icon } from '@iconify/vue';
import Dock from './ui/dock/Dock.vue';
import DockIcon from './ui/dock/DockIcon.vue';
import DockSeparator from './ui/dock/DockSeparator.vue';

</script>

<template>
  <Dock class="mb-6">
    <!-- Home -->
    <DockIcon class="group flex flex-row items-center">
      <div class="tooltip tooltip-bottom">
        <div class="tooltip-content dark:bg-white">
          <div class="animate-bounce dark:text-orange-400 -rotate-10 text-2xl font-black text-blue-600">
            Back Home</div>
        </div>
        <Icon icon="ic:baseline-home"
          class="text-blue-500 dark:text-blue-200 text-4xl opacity-70 group-hover:text-orange-500 transition-opacity"
          @click="() => $router.push('/')" />
      </div>
    </DockIcon>
    <DockSeparator />
    <!-- Blogs -->
    <DockIcon class="group flex flex-row items-center">
      <div class="tooltip tooltip-bottom">
        <div class="tooltip-content dark:bg-white">
          <div class="animate-bounce dark:text-orange-400 -rotate-10 text-2xl font-black text-blue-600">
            Blogs</div>
        </div>
        <Icon icon="ic:baseline-edit-note"
          class="text-blue-500 dark:text-blue-200 text-4xl opacity-70 group-hover:text-orange-500 transition-opacity"
          @click="() => $router.push('/blogs')" />
      </div>
    </DockIcon>
    <DockSeparator />
    <!-- Courses -->
    <DockIcon class="group flex flex-row items-center">
      <div class="tooltip tooltip-bottom">
        <div class="tooltip-content dark:bg-white">
          <div class="animate-bounce dark:text-orange-400 -rotate-10 text-2xl font-black text-blue-600">Courses</div>
        </div>
        <Icon icon="material-symbols:book-2"
          class="text-blue-500 dark:text-blue-200 text-4xl opacity-70 group-hover:text-orange-500 transition-opacity"
          @click="() => $router.push('/courses')" />
      </div>
    </DockIcon>
    <DockSeparator />
    <!-- Contact -->
    <DockIcon group flex flex-row items-center>
      <div class="tooltip tooltip-bottom">
        <div class="tooltip-content dark:bg-white">
          <div class="animate-bounce dark:text-orange-400 -rotate-10 text-2xl font-black text-green-600">Contact</div>
        </div>
        <Icon icon="mdi:email"
          class="text-green-500 dark:text-green-200 text-4xl group-hover:text-orange-500 opacity-70 transition-opacity" />
      </div>
    </DockIcon>
  </Dock>
</template>

<script setup lang="ts">
</script>