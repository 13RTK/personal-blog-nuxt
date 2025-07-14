<template>
  <div class="dark:bg-gray-800 bg-white h-full w-full theme-transition">
    <nav class="navbar sticky top-0 z-50 w-full
            bg-white/30 dark:bg-black/30 
            backdrop-filter backdrop-blur-lg
            shadow-sm text-black dark:text-white">
      <Navbar />
    </nav>

    <main class="mt-8 text-black dark:text-white dark:bg-gray-800">
      <NuxtPage />
    </main>
  </div>
</template>
