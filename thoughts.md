---
layout: default
title: 后花园
permalink: /thoughts/
---

<!-- @format -->

<div class="thoughts-container">
  <h1 class="page-title">后花园</h1>
  <p class="page-description">这里是我的随想和感悟，欢迎漫步其中</p>
  
  <div class="thoughts-grid">
    <div class="thought-card">
      <div class="thought-date">2023年10月15日</div>
      <h2 class="thought-title">秋日的思考</h2>
      <div class="thought-content">
        <p>秋天来了，树叶开始变黄，这让我想起了时间的流逝。我们总是在忙碌中度过每一天，却很少停下来思考我们真正想要的是什么。</p>
        <p>或许生活不需要那么匆忙，偶尔慢下脚步，欣赏身边的风景，感受当下的美好，也是一种生活的智慧。</p>
      </div>
      <div class="thought-tags">
        <span class="tag">生活</span>
        <span class="tag">思考</span>
        <span class="tag">秋天</span>
      </div>
    </div>
    
    <div class="thought-card">
      <div class="thought-date">2023年8月3日</div>
      <h2 class="thought-title">关于阅读的一些想法</h2>
      <div class="thought-content">
        <p>最近读了几本书，发现阅读真的是一种奇妙的体验。通过文字，我们可以跨越时空的限制，与不同时代、不同文化背景的人进行对话。</p>
        <p>阅读不仅仅是获取知识，更是一种灵魂的对话和思想的碰撞。</p>
      </div>
      <div class="thought-tags">
        <span class="tag">阅读</span>
        <span class="tag">思考</span>
      </div>
    </div>
    
    <!-- 可以添加更多随想卡片 -->
  </div>
</div>

<style>
.thoughts-container {
  padding: 20px;
  max-width: 900px;
  margin: 0 auto;
}

.page-title {
  font-size: 2.5rem;
  color: #333;
  margin-bottom: 10px;
}

.page-description {
  font-size: 1.2rem;
  color: #666;
  margin-bottom: 40px;
}

.thoughts-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(400px, 1fr));
  grid-gap: 30px;
}

.thought-card {
  background-color: #fff;
  border-radius: 10px;
  padding: 25px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  transition: transform 0.3s, box-shadow 0.3s;
}

.thought-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
}

.thought-date {
  font-size: 0.9rem;
  color: #888;
  margin-bottom: 10px;
}

.thought-title {
  font-size: 1.8rem;
  color: #333;
  margin-bottom: 15px;
}

.thought-content {
  color: #555;
  line-height: 1.6;
  margin-bottom: 20px;
}

.thought-content p {
  margin-bottom: 10px;
}

.thought-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.tag {
  display: inline-block;
  padding: 5px 12px;
  border-radius: 20px;
  background-color: #f0f0f0;
  color: #555;
  font-size: 0.85rem;
  transition: background-color 0.3s;
}

.tag:hover {
  background-color: #e0e0e0;
}

@media (max-width: 768px) {
  .thoughts-grid {
    grid-template-columns: 1fr;
  }
}
</style>
