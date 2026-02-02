---
widget: blank
headless: true
weight: 92
title: Activities
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

  <!-- 侧图轮播（你也可以放不同图片） -->
  <div class="series-carousel series-carousel-side">
    <img src="/media/uk-visits/uk-1.jpg" class="series-img active">
    <img src="/media/uk-visits/uk-2.jpg" class="series-img">
    <img src="/media/uk-visits/uk-5.jpg" class="series-img">
    <img src="/media/uk-visits/uk-7.jpg" class="series-img">
  </div>
</div>

  <div class="news-text">
    <h3>Our Lab’s Academic Visit in the UK 🇬🇧</h3>
    <p class="news-date">2026-01-18 – 2026-01-25</p>
    <p class="series-desc">
      This was a fulfilling and memorable academic visit to the UK, during which both our minds and our appetites were thoroughly satisfied. Many thanks to Prof. Hongkai Wen (University of Warwick), Prof. Tony Prescott and Prof. Chaona Chen (University of Sheffield), and Prof. Lei Zhang (University of Birmingham) for the warm welcome and lively, inspiring discussions. A highlight for all of us was touring the robotics centre and getting hands-on with the lovely MiRo robots (the ones we’re proudly holding in the photo)!
    </p>
  </div>
</div>

<div class="section-divider"></div>

<div class="news-cards">

  <!-- 新闻卡片 -->
  
  <div class="news-card">
      <img src="/media/visit-xdream.jpg" alt="sii_TopTen_singer_nitingjuntao" class="news-img">
      <div class="news-text">
        <h3>Industry Visit: Exploring Emotional Companion Robots at XDream Robotics</h3>
        <p class="news-date">2026-01-28</p>
      </div>
  </div>
  
  <!-- <div class="news-card">
      <img src="/media/academic_visit-sheffield.jpg" alt="sii_TopTen_singer_nitingjuntao" class="news-img">
      <div class="news-text">
        <h3>Academic Visit to Professor Hongkai Wen at University of Sheffield</h3>
        <p class="news-date">2026-01-20</p>
      </div>
  </div>
  
  <div class="news-card">
      <img src="/media/academic_visit-warwick.jpg" alt="sii_TopTen_singer_nitingjuntao" class="news-img">
      <div class="news-text">
        <h3>Academic Visit to Professor Hongkai Wen at University of Warwick</h3>
        <p class="news-date">2026-01-20</p>
      </div>
  </div>

  <div class="news-card">
      <img src="/media/academic_visit-birminham.jpg" alt="sii_TopTen_singer_nitingjuntao" class="news-img">
      <div class="news-text">
        <h3>Academic Visit to Professor Lei Zhang at University of Birminham</h3>
        <p class="news-date">2026-01-19</p>
      </div>
  </div> -->
  
  <div class="news-card">
      <img src="/media/sii_TopTen_singer_nitingjuntao1.jpg" alt="sii_TopTen_singer_nitingjuntao" class="news-img">
      <div class="news-text">
        <h3>Tingjuntao Ni Wins Top 10 Singer Award at SII 🏆</h3>
        <p class="news-date">2026-01-09</p>
      </div>
  </div>

  <div class="news-card">
      <img src="/media/talk_chaonachen.jpg" alt="talk_chaonachen" class="news-img">
      <div class="news-text">
        <h3>Invited Talk: Prof. Chaona Chen (University of Sheffield) on Facial Emotion Recognition in Human-Computer Interaction</h3>
        <p class="news-date">2026-01-07</p>
      </div>
  </div>

  <div class="news-card">
    <img src="/media/nacp_xuyining.jpg" alt="nacp_xuyining" class="news-img">
    <div class="news-text">
      <h3>Yining Xu Presents Poster at the 26th National Academic Conference of Psychology</h3>
      <p class="news-date">2025-11-01</p>
    </div>
  </div>

  <div class="news-card">
    <img src="/media/sii-festtech.jpg" alt="sii-festtech" class="news-img">
    <div class="news-text">
      <h3>Tingjuntao Ni and Zhenni Wang Present Poster at SII TechFest 2025</h3>
      <p class="news-date">2025-09-12</p>
    </div>
  </div>
  
  
  <div class="news-card">
    <img src="/media/lab-retreat.jpg" alt="lab-retreat" class="news-img">
    <div class="news-text">
      <h3>Lab Retreat 2025 at Zhoushan, Zhejiang</h3>
      <p class="news-date">2025-08-22</p>
    </div>
  </div>


  <div class="news-card">
    <img src="/media/lab-cartoon.jpg" alt="lab-cartoon" class="news-img">
    <div class="news-text">
      <h3>Our Lab’s Cartoon Group Photo Is Here!</h3>
      <p class="news-date">2025-06-26</p>
    </div>
  </div>

  <div class="news-card">
    <img src="media/zhenni_vss.jpg" alt="zhenni_vss" class="news-img">
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

.series-carousel {
  position: relative;
  width: 100%;
  height: 200px;
  overflow: hidden;
}

.series-img {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  opacity: 0;
  transition: opacity .5s ease;
}

.series-img.active {
  opacity: 1;
}

.series-list {
  padding-left: 18px;
  margin: 8px 0 0;
  font-size: 14px;
  color: #444;
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

