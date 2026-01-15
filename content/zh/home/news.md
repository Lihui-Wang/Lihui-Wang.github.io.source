---
widget: blank
headless: true
weight: 92
title: 活动
design:
  columns: "1"
---

<div class="news-cards">

  <!-- 新闻卡片 -->
  <div class="news-card">
      <img src="/media/sii_TopTen_singer_nitingjuntao.jpg" alt="sii_TopTen_singer_nitingjuntao" class="news-img">
      <div class="news-text">
        <h3>倪婷珺陶获得上海创智学院十佳歌手奖 🏆</h3>
        <p class="news-date">2026-01-09</p>
      </div>
  </div>

  <div class="news-card">
      <img src="/media/talk_chaonachen.jpg" alt="talk_chaonachen" class="news-img">
      <div class="news-text">
        <h3>陈超娜教授（谢菲尔德大学）做客分享：人机交互中的面部情绪识别</h3>
        <p class="news-date">2026-01-07</p>
      </div>
  </div>
  
  <div class="news-card">
    <img src="/media/nacp_xuyining.jpg" alt="nacp_xuyining" class="news-img">
    <div class="news-text">
      <h3>徐怡宁在第二十六届全国心理学学术会议上进行海报展示</h3>
      <p class="news-date">2025-11-01</p>
    </div>
  </div>
  
  <div class="news-card">
    <img src="/media/sii-festtech.jpg" alt="sii-festtech" class="news-img">
    <div class="news-text">
      <h3>倪婷珺陶和王珍妮在2025创智未来大会上进行海报展示</h3>
      <p class="news-date">2025-09-12</p>
    </div>
  </div>
  
  
  <div class="news-card">
    <img src="/media/lab-retreat.jpg" alt="lab-retreat" class="news-img">
    <div class="news-text">
      <h3>2025年实验室在浙江舟山团建</h3>
      <p class="news-date">2025-08-22</p>
    </div>
  </div>


  <div class="news-card">
    <img src="/media/lab-cartoon.jpg" alt="实验室合照漫画版" class="news-img">
    <div class="news-text">
      <h3>实验室合照卡通版！</h3>
      <p class="news-date">2025-08-15</p>
    </div>
  </div>

  <div class="news-card">
    <img src="/media/zhenni_vss.jpg" alt="zhenni_vss" class="news-img">
    <div class="news-text">
      <h3>王珍妮在2025年VSS年会上进行海报展示</h3>
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
