<template>
    <div class="slidev-layout">
      <!-- Red top bar with logo -->
      <div class="absolute top-0 left-0 right-0 bg-[#A63346] h-21 flex justify-between items-center px-8">
          <h1 class="text-white text-2xl font-bold font-calibri">{{ $frontmatter.title }}</h1>
          <img src="/polyu-small-logo.png" class="w-16 h-16" />
      </div>
      <div class="content-container">
        <slot />
      </div>

    </div>

  </template>
  
  <script setup>
  </script>
  
  <style scoped>
  .font-calibri {
    font-family: 'Calibri', sans-serif;
  }
  
  .content-container {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    min-height: calc(100vh - 5rem);
    width: 100%;
    overflow: auto;
    position: relative;
    z-index: 10;
    padding-top: 5rem;
    padding-left: 1rem;
    padding-right: 1rem;
    margin-bottom: auto;
  }

  .slidev-layout {
    display: flex;
    flex-direction: column;
    height: 100vh;
  }
  </style> 