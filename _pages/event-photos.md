---
permalink: /event-photos/
title: "Event Photos"
layout: splash
---

## Event Photos

#### Speakers giving their talks

<div class="photo-gallery">
  <div class="photo-grid">
    {% assign talk_files = "IMG_20251020_092028~2.jpg,IMG_20251020_093447~2.jpg,IMG_20251020_095850~2.jpg,IMG_20251020_111418~2.jpg,IMG_20251020_114736~2.jpg" | split: "," %}
    {% for photo in talk_files %}
      <div class="photo-item">
        <a href="/assets/images/talks/{{ photo }}" target="_blank">
          <img src="/assets/images/talks/{{ photo }}" alt="Workshop Talk" loading="lazy">
        </a>
      </div>
    {% endfor %}
  </div>
</div>

#### Handing out awards to the best submissions

<div class="photo-gallery">
  <div class="photo-grid">
    {% assign award_files = "IMG_9804.jpg,IMG_9809.jpg,IMG_9814.jpg" | split: "," %}
    {% for photo in award_files %}
      <div class="photo-item">
        <a href="/assets/images/awards/{{ photo }}" target="_blank">
          <img src="/assets/images/awards/{{ photo }}" alt="Award Ceremony" loading="lazy">
        </a>
      </div>
    {% endfor %}
  </div>
</div>

#### Other moments during the workshop

<div class="photo-gallery">
  <div class="photo-grid">
    {% assign other_files = "IMG_20251020_093839~2.jpg,IMG_20251020_101424~2.jpg,IMG_20251020_121907~2.jpg,IMG_9818~2.jpg" | split: "," %}
    {% for photo in other_files %}
      <div class="photo-item">
        <a href="/assets/images/others/{{ photo }}" target="_blank">
          <img src="/assets/images/others/{{ photo }}" alt="Workshop Moment" loading="lazy">
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

.page__content h3 {
  margin-top: 2rem;
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #e8e8e8;
}

.page__content h3:first-of-type {
  margin-top: 1.5rem;
}

.photo-gallery {
  margin: 0 0 2rem 0;
  max-width: 1400px;
}

.photo-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
  gap: 1.2rem;
  padding: 0 0 1rem 0;
}

.photo-item {
  position: relative;
  overflow: hidden;
  border-radius: 6px;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.08);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  background-color: #fff;
  aspect-ratio: 4 / 3;
}

.photo-item:hover {
  transform: translateY(-3px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

.photo-item a {
  display: block;
  text-decoration: none;
  width: 100%;
  height: 100%;
}

.photo-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  transition: opacity 0.2s ease;
}

.photo-item:hover img {
  opacity: 0.92;
}

/* Zoom icon on hover */
.photo-item a::after {
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

.photo-item:hover a::after {
  opacity: 1;
}

/* Responsive adjustments */
@media (max-width: 1200px) {
  .photo-grid {
    grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
  }
}

@media (max-width: 768px) {
  .photo-grid {
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 1rem;
  }

  .page__title {
    font-size: 1.5em !important;
  }

  .page__content h3 {
    font-size: 1.2em !important;
  }
}

@media (max-width: 480px) {
  .photo-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 0.8rem;
  }
}
</style>
