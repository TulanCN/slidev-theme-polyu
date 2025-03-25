<template>
    <div class="polyu-header">
      <img src="/logo-polyu.png" alt="PolyU Logo" class="polyu-logo" />
    </div>
    <div class="content-container">
      <div class="title-container">
        <slot />
      </div>
    </div>
    <div class="polyu-footer">
      <img src="/polyu-slogan.png" alt="Opening Minds • Shaping the Future" class="polyu-slogan" />
    </div>
</template>

<style>
.polyu-header {
  position: absolute;
  top: 0;
  left: 0;
  width: 80%;
  padding: 20px;
  background-color: white;
}

.polyu-logo {
  height: 50px;
}

.content-container {
  padding-top: 30px;
  width: 100%;
  flex-direction: column;
  justify-content: center;
  height: 100%;
}

.title-container {
  padding: 50px;
  background-color: #a6192e;
  color: white;
  margin-top: 80px;
  height: 300px;
}

/* 标题和文本的字体样式 */
.title-container h1 {
  font-family: 'Calibri', sans-serif;
  font-weight: 700;
  font-size: 2.0em;
  letter-spacing: 0.01em;
  margin-bottom: 20px;
}

.title-container h2 {
  font-family: 'Calibri', sans-serif;
  font-weight: 600;
  font-size: 1.8em;
  margin-bottom: 15px;
}

.title-container p {
  font-family: 'Calibri', sans-serif;
  font-weight: 400;
  font-size: 1.2em;
  line-height: 1.5;
}

.polyu-footer {
  position: absolute;
  bottom: 60px;
  right: 0px;
}

.polyu-slogan {
  height: 400px;
}
</style>
