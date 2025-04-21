---
layout: default
title: 学习室
permalink: /study/
---

<!-- @format -->

<div class="study-room-container">
  <h1 class="page-title">学习室</h1>
  <p class="page-description">这里记录我的学习笔记和博客文章</p>
  
  <div class="post-list-container">
    <ul class="post-list">
      {% for post in site.posts %}
        <li class="post-item">
          <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
          <h2 class="post-title">
            <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h2>
          <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
          <a href="{{ post.url | relative_url }}" class="read-more">阅读全文 →</a>
        </li>
      {% endfor %}
    </ul>
  </div>
</div>

<style>
.study-room-container {
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

.post-list-container {
  max-width: 800px;
  margin: 0 auto;
}

.post-list {
  list-style: none;
  padding: 0;
}

.post-item {
  margin-bottom: 40px;
  padding-bottom: 30px;
  border-bottom: 1px solid #eee;
}

.post-date {
  display: block;
  color: #888;
  font-size: 0.9rem;
  margin-bottom: 10px;
}

.post-title {
  margin-top: 0;
  margin-bottom: 15px;
}

.post-link {
  color: #1756a9;
  text-decoration: none;
  font-size: 1.8rem;
  transition: color 0.3s;
}

.post-link:hover {
  color: #123a6a;
}

.post-excerpt {
  color: #555;
  line-height: 1.6;
  margin-bottom: 15px;
}

.read-more {
  display: inline-block;
  color: #1756a9;
  text-decoration: none;
  font-weight: 500;
  transition: all 0.3s;
}

.read-more:hover {
  color: #123a6a;
  text-decoration: underline;
}
</style>
