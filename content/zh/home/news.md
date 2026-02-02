---
widget: blank
headless: true
weight: 92
title: 活动
design:
  columns: "1"
---

<div class="news-card series-card">
  <div class="series-media">
  <!-- 主图轮播 -->
  <div class="series-carousel series-carousel-main">
    <img src="/media/uk-visits/academic_visit-sheffield.jpg" class="series-img active">
    <img src="/media/uk-visits/academic_visit-warwick.jpg" class="series-img">
    <img src="/media/uk-visits/academic_visit-birminham.jpg" class="series-img">
    <img src="/media/uk-visits/uk-4.jpg" class="series-img">
    <img src="/media/uk-visits/uk-6.jpg" class="series-img">
  </div>

  <!-- 侧图轮播 -->
  <div class="series-carousel series-carousel-side">
    <img src="/media/uk-visits/uk-1.jpg" class="series-img active">
    <img src="/media/uk-visits/uk-2.jpg" class="series-img">
    <img src="/media/uk-visits/uk-5.jpg" class="series-img">
    <img src="/media/uk-visits/uk-7.jpg" class="series-img">
  </div>
</div>

  <div class="news-text">
    <h3>实验室英国学术之行 🇬🇧</h3>
    <p class="news-date">2026-01-18 – 2026-01-25</p>
    <p class="series-desc">
      在此次充实的学术交流中，我们的大脑和胃都十分满足（两次美味中餐功不可没😋）。非常感谢华威大学的Hongkai Wen教授，谢菲尔德大学的Tony Prescott教授和Chaona Chen教授，以及伯明翰大学的Lei Zhang教授的热情接待。在与各位学者鼓舞人心的讨论中，我们进行了个人知识库的版本升级。此行中的高光时刻莫过于参观谢菲尔德机器人中心，并与可爱的MiRo们亲切合影！
    </p>
  </div>
</div>


<div class="section-divider"></div>

<div class="news-cards">

  <!-- 新闻卡片 -->
  
  <div class="news-card">
      <img src="/media/visit-xdream.jpg" alt="sii_TopTen_singer_nitingjuntao" class="news-img">
      <div class="news-text">
        <h3>实践活动: 在炽梦科技探索情感陪伴机器人</h3>
        <p class="news-date">2026-01-28</p>
      </div>
  </div>
  
  <div class="news-card">
      <img src="/media/sii_TopTen_singer_nitingjuntao1.jpg" alt="sii_TopTen_singer_nitingjuntao" class="news-img">
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

/* ===== 特辑：左图(3/5)右文(2/5) + 左侧两列图片 ===== */
.series-card {
  flex: 0 0 100%;          /* 特辑单独占一行 */
  flex-direction: row;     /* 横向布局：左图右文 */
  align-items: stretch;
}

/* 左侧图片区：占 3/5 */
.series-card .series-media {
  flex: 3 3 0;                 /* 3/5 */
  display: grid;
  grid-template-columns: 1fr 1fr;  /* 两列图 */
  gap: 12px;
  padding: 12px;
  box-sizing: border-box;
}

/* 两个 carousel 统一样式与高度 */
.series-card .series-carousel {
  position: relative;
  width: 100%;
  height: 220px;               /* 你可调：200/220/240 */
  overflow: hidden;
  border-radius: 10px;
}

/* 右侧文字区：占 2/5 */
.series-card .news-text {
  flex: 2 2 0;                 /* 2/5 */
  padding: 16px 18px;
}

/* 列表紧凑一点 */
.series-card .series-list {
  margin-top: 6px;
  font-size: 13px;
  line-height: 1.4;
}


/* ===== 特辑与普通条目分割线 ===== */
.section-divider {
  height: 1px;
  background: #e5e5e5;
  margin: 20px 0 24px;
}

/* ===== 响应式：小屏回到上下结构 + 图片改一列 ===== */
@media (max-width: 860px) {
  .series-card {
    flex-direction: column;
  }

  .series-card .series-media,
  .series-card .news-text {
    flex: 0 0 auto;
  }

  .series-card .series-media {
    width: 100%;
    grid-template-columns: 1fr;
    padding: 0;
    gap: 0;
  }

  .series-card .series-carousel {
    height: 180px;
    border-radius: 0;
  }
}

/* 特辑标题加大 */
.series-card .news-text h3 {
  font-size: 22px;     /* 推荐 20–24 之间 */
  line-height: 1.25;
  margin-bottom: 10px;
}

/* 轮播图片叠放与显隐控制（你当前缺少这一段） */
.series-card .series-img {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  opacity: 0;
  transition: opacity .4s ease;
}

.series-card .series-img.active {
  opacity: 1;
}

/* 特辑正文描述 */
.series-card .series-desc {
  margin-top: 6px;
  font-size: 13px;      /* 和你原来 list 一致 */
  line-height: 1.5;
  color: #444;
}

</style>

<script>
(function () {
  const card = document.querySelector('.series-card');
  if (!card) return;

  const carousels = card.querySelectorAll('.series-carousel');

  carousels.forEach((carousel, i) => {
    const imgs = carousel.querySelectorAll('.series-img');
    if (imgs.length <= 1) return;

    let idx = 0;
    const delay = i * 1500;   // 第二列延迟 1.5s

    setTimeout(() => {
      setInterval(() => {
        imgs[idx].classList.remove('active');
        idx = (idx + 1) % imgs.length;
        imgs[idx].classList.add('active');
      }, 4000);
    }, delay);
  });
})();
</script>

