<template>
  <span :class="`loading loading-infinity loading-${size || 'xl'}`"></span>
</template>

<script setup lang="ts">
defineProps<{
  size?: "xl" | "lg" | "md" | "sm" | "xs";
}>();
</script>