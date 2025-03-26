<template>
    <div class="slidev-layout">
      <!-- Red top bar with logo -->
      <div class="absolute top-0 left-0 right-0 bg-[#A63346] h-21 flex justify-between items-center px-8">
          <h1 class="text-white text-2xl font-bold font-calibri">Contents</h1>
          <img src="/polyu-small-logo.png" class="w-16 h-16" />
      </div>
    
      <!-- Content section with items -->
      <div class="content-grid">
        <div v-for="(item, index) in contentItems" :key="index" class="content-item">
          <div class="item-title flex items-center mb-1">
            <h2 class="text-3xl font-bold text-teal-500">{{ index + 1 }}. <span class="ml-2">{{ item.title }}</span></h2>
          </div>
        </div>
      </div>
    </div>

  </template>
  
  <script setup>
  import { computed } from 'vue'

  // 从前置内容中获取内容项目
  const contentItems = computed(() => {
    // 默认从 frontmatter 中获取 contentItems
    // 用户可以在 markdown 中这样定义：
    // ---
    // contentItems:
    //   - title: "介绍"
    //     description: "项目背景和目标"
    //   - title: "系统设计"
    //     description: "架构和技术栈"
    // ---
    return $frontmatter.contentItems || []
  })
  </script>
  
  <style scoped>
  .font-calibri {
    font-family: 'Calibri', sans-serif;
  }
  
  .content-container {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    width: 100%;
    overflow: hidden;
    position: relative;
    z-index: 10;
    padding-top: 2rem;
  }

  .content-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem 4rem;
    max-width: 80%;
    margin: 0 auto;
    margin-top: 6rem;
  }

  .content-item {
    margin-bottom: 2rem;
  }

  .item-title {
    color: #20B2AA;
  }

  @media (max-width: 768px) {
    .content-grid {
      grid-template-columns: 1fr;
    }
  }
  </style> 