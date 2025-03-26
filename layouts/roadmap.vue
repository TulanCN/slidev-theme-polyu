<template>
  <div class="slidev-layout roadmap">
    <!-- Red top bar with logo -->
    <div class="absolute top-0 left-0 right-0 bg-[#A63346] h-21 flex justify-end items-center px-8">
      <img src="/polyu-small-logo.png" class="w-16 h-16" />
    </div>

    <!-- Main content -->
    <div class="flex flex-col items-center justify-center h-full">
      <!-- Large number -->
      <div class="text-9xl font-bold text-teal-500 mb-8">
        {{ $frontmatter.number }}
      </div>
      
      <!-- Title -->
      <div class="text-6xl text-teal-500">
        {{ $frontmatter.title }}
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.roadmap {
  @apply p-0;
  background-color: white;
}
</style> 