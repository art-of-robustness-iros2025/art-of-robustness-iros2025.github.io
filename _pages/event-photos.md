---
permalink: /event-photos/
title: "Event Photos"
classes: wide
layout: single
---

## Workshop Event Gallery

A collection of photos from the IROS 2025 Workshop on "The Art of Robustness: Surviving Failures in Robotics" held on October 20, 2025, in Hangzhou, China.

### Invited Talks

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

### Award Ceremony

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

### Other Moments

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
.photo-gallery {
  margin: 2rem 0 3rem 0;
}

.photo-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 1.5rem;
  padding: 1rem 0;
}

.photo-item {
  position: relative;
  overflow: hidden;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  background-color: #f5f5f5;
}

.photo-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.2);
}

.photo-item a {
  display: block;
  text-decoration: none;
}

.photo-item img {
  width: 100%;
  height: auto;
  display: block;
  transition: opacity 0.3s ease;
}

.photo-item:hover img {
  opacity: 0.9;
}

/* Zoom icon on hover */
.photo-item a::after {
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

.photo-item:hover a::after {
  opacity: 1;
}

/* Section headings */
h3 {
  margin-top: 2.5rem;
  margin-bottom: 1rem;
  padding-bottom: 0.5rem;
  border-bottom: 2px solid #e0e0e0;
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .photo-grid {
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 1rem;
  }
}

@media (max-width: 480px) {
  .photo-grid {
    grid-template-columns: 1fr;
  }
}
</style>
