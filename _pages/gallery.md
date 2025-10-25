---
permalink: /gallery/
title: "Poster Gallery"
classes: wide
layout: single
---

## Workshop Poster Gallery

A collection of posters presented at the IROS 2025 Workshop on "The Art of Robustness: Surviving Failures in Robotics" held on October 20, 2025, in Hangzhou, China.

<div class="poster-gallery">
  <div class="poster-grid">
    {% assign poster_files = "IMG_20251020_100000.jpg,IMG_20251020_100013.jpg,IMG_20251020_100059.jpg,IMG_20251020_100112.jpg,IMG_20251020_100127.jpg,IMG_20251020_100133.jpg,IMG_20251020_100459.jpg,IMG_20251020_100521.jpg,IMG_20251020_100529.jpg,IMG_20251020_100545.jpg,IMG_20251020_100613.jpg,IMG_20251020_100623.jpg,IMG_20251020_101239.jpg,IMG_20251020_101246.jpg" | split: "," %}
    {% for poster in poster_files %}
      <div class="poster-item">
        <a href="/assets/images/posters/{{ poster }}" data-lightbox="posters" data-title="Workshop Poster">
          <img src="/assets/images/posters/{{ poster }}" alt="Workshop Poster" loading="lazy">
        </a>
      </div>
    {% endfor %}
  </div>
</div>

<style>
.poster-gallery {
  margin: 2rem 0;
}

.poster-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 1.5rem;
  padding: 1rem 0;
}

.poster-item {
  position: relative;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  background-color: #f5f5f5;
}

.poster-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.2);
}

.poster-item a {
  display: block;
  text-decoration: none;
}

.poster-item img {
  width: 100%;
  height: auto;
  display: block;
  transition: opacity 0.3s ease;
}

.poster-item:hover img {
  opacity: 0.9;
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .poster-grid {
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 1rem;
  }
}

@media (max-width: 480px) {
  .poster-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<!-- Lightbox functionality using CSS only -->
<style>
.poster-item a::after {
  content: '🔍';
  position: absolute;
  top: 10px;
  right: 10px;
  background: rgba(255, 255, 255, 0.9);
  padding: 5px 10px;
  border-radius: 4px;
  opacity: 0;
  transition: opacity 0.3s ease;
  font-size: 1.2rem;
}

.poster-item:hover a::after {
  opacity: 1;
}
</style>
