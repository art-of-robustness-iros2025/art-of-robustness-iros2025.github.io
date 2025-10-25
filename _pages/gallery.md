---
permalink: /gallery/
title: "Poster Gallery"
layout: splash
---

## Poster Gallery

<div class="poster-gallery">
  <div class="poster-grid">
    {% assign poster_files = "IMG_20251020_100000.jpg,IMG_20251020_100013.jpg,IMG_20251020_100059.jpg,IMG_20251020_100112.jpg,IMG_20251020_100127.jpg,IMG_20251020_100133.jpg,IMG_20251020_100459.jpg,IMG_20251020_100521.jpg,IMG_20251020_100529.jpg,IMG_20251020_100545.jpg,IMG_20251020_100613.jpg,IMG_20251020_100623.jpg,IMG_20251020_101239.jpg,IMG_20251020_101246.jpg" | split: "," %}
    {% for poster in poster_files %}
      <div class="poster-item">
        <a href="/assets/images/posters/{{ poster }}" target="_blank">
          <img src="/assets/images/posters/{{ poster }}" alt="Workshop Poster" loading="lazy">
        </a>
      </div>
    {% endfor %}
  </div>
</div>

<style>
/* Layout styling for gallery pages */
.page {
  max-width: 100% !important;
  padding-left: 1rem !important;
  padding-right: 1rem !important;
}

.page__inner-wrap {
  max-width: 1400px !important;
  margin-left: auto !important;
  margin-right: auto !important;
}

.poster-gallery {
  margin: 0 auto;
  max-width: 1400px;
  padding: 0;
}

.poster-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
  gap: 1.2rem;
  padding: 0;
}

.poster-item {
  position: relative;
  overflow: hidden;
  border-radius: 6px;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.08);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  background-color: #fff;
  aspect-ratio: 3 / 4;
}

.poster-item:hover {
  transform: translateY(-3px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

.poster-item a {
  display: block;
  text-decoration: none;
  width: 100%;
  height: 100%;
}

.poster-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  transition: opacity 0.2s ease;
}

.poster-item:hover img {
  opacity: 0.92;
}

/* Zoom icon on hover */
.poster-item a::after {
  content: '🔍';
  position: absolute;
  top: 8px;
  right: 8px;
  background: rgba(255, 255, 255, 0.95);
  padding: 4px 8px;
  border-radius: 4px;
  opacity: 0;
  transition: opacity 0.2s ease;
  font-size: 1rem;
  pointer-events: none;
}

.poster-item:hover a::after {
  opacity: 1;
}

/* Responsive adjustments */
@media (max-width: 1200px) {
  .poster-grid {
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  }
}

@media (max-width: 768px) {
  .poster-grid {
    grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
    gap: 1rem;
  }

  .page__title {
    font-size: 1.5em !important;
  }
}

@media (max-width: 480px) {
  .poster-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 0.8rem;
  }
}
</style>
