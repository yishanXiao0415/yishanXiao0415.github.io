---
layout: default
title: 传声室
permalink: /message/
---

<!-- @format -->

<div class="message-room-container">
  <h1 class="page-title">传声室</h1>
  <p class="page-description">欢迎在此留下你的想法和建议</p>
  
  <div class="message-form-container">
    <form class="message-form" action="https://formspree.io/f/your-formspree-id" method="POST">
      <div class="form-group">
        <label for="name">您的昵称</label>
        <input type="text" id="name" name="name" required>
      </div>
      
      <div class="form-group">
        <label for="email">您的邮箱</label>
        <input type="email" id="email" name="email" required>
      </div>
      
      <div class="form-group">
        <label for="message">留言内容</label>
        <textarea id="message" name="message" rows="6" required></textarea>
      </div>
      
      <button type="submit" class="submit-btn">发送留言</button>
    </form>
  </div>
  
  <div class="messages-container">
    <h2 class="messages-title">访客留言</h2>
    <div class="messages-list">
      <p class="message-placeholder">留言功能正在建设中，敬请期待...</p>
      <!-- 留言列表将在后续通过JavaScript加载 -->
    </div>
  </div>
</div>

<style>
.message-room-container {
  padding: 20px;
  max-width: 800px;
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

.message-form-container {
  background-color: #f9f9f9;
  padding: 30px;
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0,0,0,0.1);
  margin-bottom: 50px;
}

.form-group {
  margin-bottom: 20px;
}

.form-group label {
  display: block;
  margin-bottom: 8px;
  font-weight: 500;
  color: #444;
}

.form-group input,
.form-group textarea {
  width: 100%;
  padding: 12px;
  border: 1px solid #ddd;
  border-radius: 5px;
  font-size: 16px;
  font-family: inherit;
}

.form-group textarea {
  resize: vertical;
}

.form-group input:focus,
.form-group textarea:focus {
  outline: none;
  border-color: #1756a9;
  box-shadow: 0 0 0 2px rgba(23, 86, 169, 0.2);
}

.submit-btn {
  background-color: #1756a9;
  color: white;
  border: none;
  padding: 12px 25px;
  border-radius: 5px;
  font-size: 16px;
  font-weight: 500;
  cursor: pointer;
  transition: background-color 0.3s;
}

.submit-btn:hover {
  background-color: #123a6a;
}

.messages-container {
  margin-top: 40px;
}

.messages-title {
  font-size: 1.8rem;
  color: #333;
  margin-bottom: 20px;
  padding-bottom: 10px;
  border-bottom: 1px solid #eee;
}

.message-placeholder {
  color: #888;
  font-style: italic;
  text-align: center;
  padding: 30px 0;
}
</style>
