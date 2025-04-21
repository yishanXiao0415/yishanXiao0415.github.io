---
layout: default
title: 博物馆
permalink: /gallery/
---

<!-- @format -->

<div class="gallery-container">
  <h1 class="page-title">博物馆</h1>
  <p class="page-description">收藏照片、明信片和精彩瞬间</p>
  
  <div class="gallery-filter">
    <button class="filter-btn active" data-filter="all">全部</button>
    <button class="filter-btn" data-filter="photos">照片</button>
    <button class="filter-btn" data-filter="postcards">明信片</button>
    <button class="filter-btn" data-filter="artwork">艺术作品</button>
  </div>
  
  <div class="gallery-grid">
    <!-- 示例图片，实际使用时替换为您自己的图片 -->
    <div class="gallery-item" data-category="photos">
      <div class="gallery-item-inner">
        <img src="https://via.placeholder.com/400x300" alt="照片示例">
        <div class="gallery-item-overlay">
          <h3>照片标题</h3>
          <p>2023年8月15日</p>
        </div>
      </div>
    </div>
    
    <div class="gallery-item" data-category="postcards">
      <div class="gallery-item-inner">
        <img src="https://via.placeholder.com/400x300" alt="明信片示例">
        <div class="gallery-item-overlay">
          <h3>明信片标题</h3>
          <p>来自北京</p>
        </div>
      </div>
    </div>
    
    <div class="gallery-item" data-category="artwork">
      <div class="gallery-item-inner">
        <img src="https://via.placeholder.com/400x300" alt="艺术作品示例">
        <div class="gallery-item-overlay">
          <h3>艺术作品标题</h3>
          <p>水彩画</p>
        </div>
      </div>
    </div>
    
    <!-- 更多图片项... -->
  </div>
</div>

<style>
.gallery-container {
  padding: 20px;
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

.gallery-filter {
  display: flex;
  justify-content: center;
  margin-bottom: 30px;
  flex-wrap: wrap;
}

.filter-btn {
  background: none;
  border: none;
  padding: 10px 20px;
  margin: 0 5px 10px;
  font-size: 16px;
  cursor: pointer;
  border-radius: 30px;
  color: #333;
  transition: all 0.3s;
}

.filter-btn:hover, .filter-btn.active {
  background-color: #1756a9;
  color: white;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  grid-gap: 20px;
}

.gallery-item {
  overflow: hidden;
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0,0,0,0.1);
}

.gallery-item-inner {
  position: relative;
}

.gallery-item img {
  width: 100%;
  height: auto;
  display: block;
  transition: transform 0.5s;
}

.gallery-item:hover img {
  transform: scale(1.05);
}

.gallery-item-overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: rgba(0, 0, 0, 0.7);
  color: white;
  padding: 15px;
  transform: translateY(100%);
  transition: transform 0.3s;
}

.gallery-item:hover .gallery-item-overlay {
  transform: translateY(0);
}

.gallery-item-overlay h3 {
  margin: 0 0 5px;
  font-size: 18px;
}

.gallery-item-overlay p {
  margin: 0;
  font-size: 14px;
  opacity: 0.8;
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function() {
  const filterButtons = document.querySelectorAll('.filter-btn');
  const galleryItems = document.querySelectorAll('.gallery-item');
  
  filterButtons.forEach(button => {
    button.addEventListener('click', function() {
      // 移除所有按钮的active类
      filterButtons.forEach(btn => btn.classList.remove('active'));
      
      // 给当前点击的按钮添加active类
      this.classList.add('active');
      
      // 获取过滤类别
      const filterValue = this.getAttribute('data-filter');
      
      // 过滤图片
      galleryItems.forEach(item => {
        if (filterValue === 'all' || item.getAttribute('data-category') === filterValue) {
          item.style.display = 'block';
        } else {
          item.style.display = 'none';
        }
      });
    });
  });
});
</script>
