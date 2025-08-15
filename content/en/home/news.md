---
widget: blank
headless: true
weight: 92
title: Activities
design:
  columns: "1"
---

<div class="news-cards">

  <!-- 新闻卡片 -->
  <div class="news-card">
    <img src="/media/lab-cartoon.jpg" alt="lab-cartoon" class="news-img">
    <div class="news-text">
      <h3>Our Lab’s Cartoon Group Photo Is Here!</h3>
      <p class="news-date">2025-08-15</p>
    </div>
  </div>

  <div class="news-card">
    <img src="/media/zhenni_vss.jpg" alt="zhenni_vss" class="news-img">
    <div class="news-text">
      <h3>Zhenni Wang Presents Poster at VSS 2025</h3>
      <p class="news-date">2025-05-18</p>
    </div>
  </div>

</div>

<style>
.news-cards {
  display: flex;
  flex-wrap: wrap;
  gap: 24px;
}
.news-card {
  flex: 0 0 calc(25% - 24px);
  background: #fff;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.08);
  overflow: hidden;
  display: flex;
  flex-direction: column;
  transition: transform .15s ease;
}
.news-card:hover {
  transform: translateY(-4px);
}
.news-img {
  width: 100%;
  aspect-ratio: 4 / 3;
  object-fit: cover;
}
.news-text {
  padding: 12px 16px;
}
.news-text h3 {
  margin: 0 0 8px;
  font-size: 16px;
  font-weight: 600;
  color: #000;
}
.news-date {
  margin: 0;
  font-size: 14px;
  color: #666;
}
/* 移动端 2列 */
@media (max-width: 860px) {
  .news-card {
    flex: 0 0 calc(50% - 24px);
  }
}
/* 小屏 1列 */
@media (max-width: 500px) {
  .news-card {
    flex: 0 0 100%;
  }
}
</style>
