---
layout: home
title: 首页
permalink: /
---

<!-- @format -->

<div class="welcome-container">
  <div class="welcome-header">
    <div class="datetime-container">
      <div id="current-time" class="current-time">00:00</div>
      <div id="current-date" class="current-date">2023年1月1日 星期一</div>
    </div>
    <div class="welcome-message">
      <h1>WELCOME TO yishan's WORLD</h1>
    </div>
    <div class="start-button-container">
      <a href="/map" class="start-button">START</a>
    </div>
  </div>
</div>

<style>
.welcome-container {
  height: 100vh;
  width: 100%;
  background-image: url('/assets/images/1.png');
  background-size: cover;
  background-position: center;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
}

.welcome-header {
  text-align: center;
  color: #fff;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
}

.datetime-container {
  margin-bottom: 30px;
}

.current-time {
  font-size: 7rem;
  font-weight: 700;
  line-height: 1;
  margin-bottom: 10px;
}

.current-date {
  font-size: 1.5rem;
}

.welcome-message h1 {
  font-size: 2.5rem;
  margin-bottom: 50px;
  letter-spacing: 2px;
}

.start-button-container {
  margin-top: 40px;
}

.start-button {
  display: inline-block;
  padding: 15px 50px;
  background-color: rgba(255, 255, 255, 0.2);
  color: #fff;
  text-decoration: none;
  border: 2px solid #fff;
  font-size: 1.2rem;
  font-weight: bold;
  border-radius: 30px;
  transition: all 0.3s ease;
  letter-spacing: 2px;
}

.start-button:hover {
  background-color: rgba(255, 255, 255, 0.4);
  transform: translateY(-3px);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
}
</style>

<script>
function updateDateTime() {
  const now = new Date();
  
  // 更新时间
  const hours = String(now.getHours()).padStart(2, '0');
  const minutes = String(now.getMinutes()).padStart(2, '0');
  document.getElementById('current-time').textContent = `${hours}:${minutes}`;
  
  // 更新日期
  const year = now.getFullYear();
  const month = now.getMonth() + 1;
  const day = now.getDate();
  const weekdays = ['日', '一', '二', '三', '四', '五', '六'];
  const weekday = weekdays[now.getDay()];
  document.getElementById('current-date').textContent = `${year}年${month}月${day}日 星期${weekday}`;
}

// 初始更新并设置每秒更新一次
updateDateTime();
setInterval(updateDateTime, 1000);
</script>
