<!-- @format -->

<!--
 * @Author: SOMMER
 * @Date: 2025-04-20 19:32:13
 * @LastEditTime: 2025-04-21 00:22:20
 * @FilePath: \blog\about.md
-->

---

layout: default
title: 小窝
permalink: /about/

---

<div class="about-container">
  <div class="about-header">
    <div class="avatar-container">
      <img src="https://via.placeholder.com/150" alt="头像" class="avatar">
    </div>
    <h1 class="about-title">关于我</h1>
    <p class="about-subtitle">欢迎来到我的小窝</p>
  </div>
  
  <div class="about-content">
    <div class="about-section">
      <h2 class="section-title">个人简介</h2>
      <div class="section-content">
        <p>你好，我是yishan，欢迎来到我的博客！</p>
        <p>这里是我记录生活、学习和思考的地方。我喜欢阅读、写作和探索新事物。</p>
        <p>希望我的博客能给你带来一些启发或者放松的时刻。</p>
      </div>
    </div>
    
    <div class="about-section">
      <h2 class="section-title">兴趣爱好</h2>
      <div class="section-content">
        <div class="interests-grid">
          <div class="interest-item">
            <i class="fa fa-book"></i>
            <span>阅读</span>
          </div>
          <div class="interest-item">
            <i class="fa fa-music"></i>
            <span>音乐</span>
          </div>
          <div class="interest-item">
            <i class="fa fa-camera"></i>
            <span>摄影</span>
          </div>
          <div class="interest-item">
            <i class="fa fa-paint-brush"></i>
            <span>绘画</span>
          </div>
          <div class="interest-item">
            <i class="fa fa-code"></i>
            <span>编程</span>
          </div>
          <div class="interest-item">
            <i class="fa fa-plane"></i>
            <span>旅行</span>
          </div>
        </div>
      </div>
    </div>
    
    <div class="about-section">
      <h2 class="section-title">联系方式</h2>
      <div class="section-content">
        <div class="contact-item">
          <i class="fa fa-envelope"></i>
          <span>邮箱：your-email@example.com</span>
        </div>
        <div class="contact-item">
          <i class="fa fa-github"></i>
          <span>GitHub：<a href="https://github.com/your-github-username" target="_blank">your-github-username</a></span>
        </div>
      </div>
    </div>
  </div>
  
  <div class="friends-links">
    <h2 class="section-title">友情链接</h2>
    <div class="friends-grid">
      <a href="#" class="friend-item" target="_blank">
        <img src="https://via.placeholder.com/50" alt="朋友头像">
        <span>朋友博客1</span>
      </a>
      <a href="#" class="friend-item" target="_blank">
        <img src="https://via.placeholder.com/50" alt="朋友头像">
        <span>朋友博客2</span>
      </a>
      <a href="#" class="friend-item" target="_blank">
        <img src="https://via.placeholder.com/50" alt="朋友头像">
        <span>朋友博客3</span>
      </a>
      <!-- 可以添加更多友情链接 -->
    </div>
  </div>
</div>

<style>
.about-container {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}

.about-header {
  text-align: center;
  margin-bottom: 50px;
}

.avatar-container {
  margin-bottom: 20px;
}

.avatar {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
  border: 5px solid #fff;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

.about-title {
  font-size: 2.5rem;
  color: #333;
  margin-bottom: 10px;
}

.about-subtitle {
  font-size: 1.2rem;
  color: #666;
}

.about-section {
  margin-bottom: 40px;
}

.section-title {
  font-size: 1.8rem;
  color: #333;
  margin-bottom: 20px;
  padding-bottom: 10px;
  border-bottom: 1px solid #eee;
}

.section-content {
  color: #555;
  line-height: 1.6;
}

.section-content p {
  margin-bottom: 15px;
}

.interests-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
  grid-gap: 20px;
}

.interest-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 15px;
  background-color: #f9f9f9;
  border-radius: 10px;
  transition: transform 0.3s, background-color 0.3s;
}

.interest-item:hover {
  transform: translateY(-5px);
  background-color: #f0f0f0;
}

.interest-item i {
  font-size: 28px;
  color: #1756a9;
  margin-bottom: 10px;
}

.contact-item {
  display: flex;
  align-items: center;
  margin-bottom: 15px;
}

.contact-item i {
  font-size: 20px;
  color: #1756a9;
  margin-right: 15px;
  width: 25px;
  text-align: center;
}

.contact-item a {
  color: #1756a9;
  text-decoration: none;
  transition: color 0.3s;
}

.contact-item a:hover {
  color: #123a6a;
  text-decoration: underline;
}

.friends-links {
  margin-top: 60px;
}

.friends-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
  grid-gap: 20px;
}

.friend-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-decoration: none;
  color: #333;
  padding: 15px;
  background-color: #f9f9f9;
  border-radius: 10px;
  transition: transform 0.3s, background-color 0.3s;
}

.friend-item:hover {
  transform: translateY(-5px);
  background-color: #f0f0f0;
}

.friend-item img {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 10px;
}
</style>
