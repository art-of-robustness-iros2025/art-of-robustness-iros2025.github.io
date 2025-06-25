---
permalink: /
layout: splash

sponsors:
  - url: https://eng.bigai.ai/
    image_path: /assets/images/sponsors/BIGAI.png
    alt: "BIGAI"
  - url: https://www.lejurobot.com/
    image_path: /assets/images/sponsors/leju_robotics.png
    alt: "LEJU Robotics"
  - url: https://www.microsoft.com/en-us/research/group/microsoft-research-asia-tokyo/
    image_path: /assets/images/sponsors/microsoft.png
    alt: "Microsoft Research Asia Tokyo"
  - url: https://www.jst.go.jp/moonshot/en/program/goal3/
    image_path: /assets/images/sponsors/moonshot.png
    alt: "Moonshot Research and Development Program Goal3"
  - url: https://www.jst.go.jp/EN/
    image_path: /assets/images/sponsors/jst.png
    alt: "Japan Science and Technology Agency (JST)"
invited_speakers:
  - name: "Prof. Kensuke Harada"
    affiliation: "Osaka University"
    image_path: /assets/images/invited_speakers/Kensuke Harada.png
    topic: "Topic: Realizing robust motion planning for robotic manipulation tasks"
  - name: "Prof. Nick Hawes"
    affiliation: "University of Oxford"
    image_path: /assets/images/invited_speakers/Nick Hawes.jpeg
    topic: "Topic: Robustness through Planning in Long-term Autonomous Deployments"
  - name: "Dr. Xiaokun Leng"
    affiliation: "LEJU Robotics"
    image_path: /assets/images/invited_speakers/Xiaokun Leng.jpeg
    topic: "Topic: Development of Humanoid Robot Technology and its Industrialization"
  - name: "Dr. Sylvain Calinon"
    affiliation: "Idiap Research Institute, EPFL, Switzerland"
    image_path: /assets/images/invited_speakers/Sylvain Calinon.jpeg
    topic: "Topic: Exploiting Geometric Approaches and Ergodic Control for Robust Manipulation"
  - name: "Prof. Dimitrios Kanoulas"
    affiliation: "University College London"
    image_path: /assets/images/invited_speakers/DKanoulas-2024-sq.png
    topic: "The Good, the Bad, and the Ugly: Robustness of Robots that have Limbs"
  - name: "Dr. Jiaolong Yang"
    affiliation: "Microsoft Research Asia"
    image_path: /assets/images/invited_speakers/Jiaolong_Yang.png
    topic: "Topic: TBD"
organizers:
  - name: "Jiayi Wang"
    affiliation: "Beijing Institute for General Artificial Intelligence (BIGAI)"
    image_path: /assets/images/organizers/jiayi.jpeg
  - name: "Namiko Saito"
    affiliation: "Microsoft Research Asia Tokyo"
    image_path: /assets/images/organizers/namiko.jpeg
  - name: "Henrique Ferrolho"
    affiliation: "Address Robotics Ltd, London, UK"
    image_path: /assets/images/organizers/henrique.jpg
  - name: "Sethu Vijayakumar"
    affiliation: "The University of Edinburgh"
    image_path: /assets/images/organizers/sethu.png
  - name: "Adrian Röfer"
    affiliation: "University of Freiburg"
    image_path: /assets/images/organizers/adrian.jpeg
  # - name: "Russell Buchanan"
  #   affiliation: "University of Waterloo"
  #   image_path: /assets/images/organizers/russell.jpeg
  - name: Yue Gao
    affiliation: "Shanghai Jiaotong University"
    image_path: /assets/images/organizers/yue.jpeg
  - name: Hangxin Liu
    affiliation: "Beijing Institute for General Artificial Intelligence (BIGAI)"
    image_path: /assets/images/organizers/hangxin.jpg
  - name: Yao Su
    affiliation: "Beijing Institute for General Artificial Intelligence (BIGAI)"
    image_path: /assets/images/organizers/yao.jpeg
  - name: Song-Chun Zhu
    affiliation: "BIGAI, Peking University, Tsinghua University"
    image_path: /assets/images/organizers/SongchunZhu.jpg
    
gallery:
  - url: /assets/images/unsplash-gallery-image-1.jpg
    image_path: /assets/images/unsplash-gallery-image-1-th.jpg
    alt: "placeholder image 1"
    title: "Image 1 title caption"
  - url: /assets/images/unsplash-gallery-image-2.jpg
    image_path: /assets/images/unsplash-gallery-image-2-th.jpg
    alt: "placeholder image 2"
    title: "Image 2 title caption"
  - url: /assets/images/unsplash-gallery-image-3.jpg
    image_path: /assets/images/unsplash-gallery-image-3-th.jpg
    alt: "placeholder image 3"
    title: "Image 3 title caption"
---
<!-- 
**Disclaimer:** This workshop is not yet confirmed. We are working on our proposal submission.
{: .notice--danger}

**Warning:** This website is under construction.
{: .notice--warning} -->

<!-- # {{ site.title }} -->

<style>
  h1:first-of-type {
    margin-top: 50px;  /* Add space above the title */
    padding-top: 20px; /* Additional padding if needed */
  }
</style>

# The Art of Robustness: Surviving Failures in Robotics

*Multi-functional Hall B, Hangzhou International Expo Center, Hangzhou, China*

*October 20, 2025, 8:30 AM – 12:30 PM*

## Introduction

In recent years, we have seen significant advancements in robotic systems. 
Humanoid robots can perform complex tasks, mobile manipulators show promise in logistics and industrial applications, and exoskeletons enhance human capabilities.
However, deploying robots in real-world applications still remains challenging. 
**A primary bottleneck is the occurrence of failures that compromise the robustness of robotic systems**, limiting their reliability in practical scenarios. 
Below is a video showing robot failures experienced by the workshop organizers, 
illustrating the impact of these failures in real-world settings.

<div class="video-wrapper">
  <iframe width="720" height="405" src="https://www.youtube.com/embed/fPZR2p4dFhE?autoplay=1&mute=1&loop=1&playlist=fPZR2p4dFhE" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

<style>
  .video-wrapper {
    max-width: 1000px; /* Adjust the width as needed */
    height: auto; /* Adjust the height as needed */
    margin: 0 auto; /* Center the video */
    padding-bottom: 20px; /* Reduce the gap after the video */
  }
</style>

The primary objective of this workshop is to provide a platform for **discussing the key challenges that lead
to failures in robots**, such as perceptual noise, uncertainty in model-based methods, limited generalizability
in learning-based methods, and exploring **innovative solutions to mitigate these issues, thereby improving the
robustness of robotic systems**. Additionally, the workshop will also feature **practical aspects** often overlooked in academic papers, e.g., system integration and debugging processes to address failures.
The workshop will bring together world-renowned researchers and practitioners
from diverse fields, including whole-body model-based control, robot learning, perception and sensing, system engineering, to share
their insights and experiences. The workshop will feature invited talks, poster sessions, and panel discussions,
offering attendees a comprehensive understanding on robustness challenges in robotics and highlight the latest
advancements and strategies for addressing these obstacles.

## Topics of Dicussion and Interest

<div class="gallery">
  <div class="gallery-item">
    <img src="/assets/images/gallery/fundamental_algorithms.webp" alt="Fundamental Algorithms">
    <h3>Fundamental Algorithms</h3>
    <ul style="text-align: left; padding-left: 30px; font-size: 1.0em; line-height: 1.2;">
      <li>Model-based and learning-based methods, and combinations of them</li>
      <li>Scalability, generalization, and adaptability</li>
      <li>Real-time computation</li>
      <li>Perception and sensing techniques</li>
      <li>Failure recovery algorithms</li>
    </ul>  
</div>
  <div class="gallery-item">
    <img src="/assets/images/gallery/system_engineering.webp" alt="Real-World Implementation">
    <h3>Real-World Implementation</h3>
    <ul style="text-align: left; padding-left: 30px; font-size: 1.0em; line-height: 1.2;">
      <li>Hardware design</li>
      <li>Software engineering and system integration</li>
      <li>Sim-to-real transfer</li>
      <li>Evaluation and certification</li>
    </ul>  </div>
  <div class="gallery-item">
    <img src="/assets/images/gallery/practical_aspects.webp" alt="Practical Aspects">
    <h3>Practical Aspects</h3>
    <ul style="text-align: left; padding-left: 30px; font-size: 1.0em; line-height: 1.2;">
      <li>Nitty-gritty twists often overlooked in academic papers</li>
      <li>Debugging process to address failures</li>
      <li>Attitude and mindset when dealing with failures</li>
    </ul>
  </div>
</div>

<style>
.gallery {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  gap: 20px;
}

.gallery-item {
  text-align: center;
  max-width: 375px;
}

.gallery-item img {
  width: 100%;
  height: auto;
  border-radius: 8px;
}

.gallery-item h3 {
  margin: 10px 0 5px;
  font-size: 1.2em;
}

.gallery-item p {
  font-size: 0.9em;
  color: #666;
}
</style>

## Invited Speakers

<div class="invited-speakers">
  <ul class="speaker-list">
    {% for speaker in page.invited_speakers %}
      <li class="speaker-item">
        <img src="{{ speaker.image_path }}" alt="{{ speaker.name }}" class="speaker-img">
        <h3 class="speaker-name">{{ speaker.name }}</h3>
        <p class="speaker-affiliation">{{ speaker.affiliation }}</p>
        <p class="speaker-topic">{{ speaker.topic }}</p>
      </li>
    {% endfor %}
  </ul>
</div>

<style>
  .speaker-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: left;
    gap: 20px;
    list-style-type: none;
    padding: 0;
  }
  .speaker-item {
    flex: 1 1 calc(30% - 40px); /* Adjust the size as needed */
    text-align: center;
  }
  .speaker-img {
    width: 150px; /* Adjust the width as needed */
    height: 150px; /* Set the height to match the width */
    border-radius: 50%; /* Make the image circular */
    object-fit: cover; /* Ensure the image covers the area without distortion */
  }
  .speaker-name {
    font-size: 1.0em; /* Adjust the font size as needed */
  }
  .speaker-affiliation {
    font-size: 1.0em; /* Adjust the font size as needed */
  }
  .speaker-topic {
    font-size: 1.0em; /* Adjust the font size as needed */
  }
</style>

## Call for Posters

We invite researchers to submit short papers on preliminary results, ongoing works, and demos relevant to the workshop via [this Link](https://openreview.net/group?id=IEEE.org/IROS/2025/Workshop/TARo#tab-your-consoles) in the form of a short papers (2-4 pages, excluding references).

### Important Dates

- **Submission Deadline**: 5th September 2025
- **Notification**: 20th September 2025

## Organizers

<div class="organizers">
  <ul class="organizer-list">
    {% for organizer in page.organizers %}
      <li class="organizer-item">
        <img src="{{ organizer.image_path }}" alt="{{ organizer.name }}" class="organizer-img">
        <h3 class="organizer-name">{{ organizer.name }}</h3>
        <p class="organizer-affiliation">{{ organizer.affiliation }}</p>
      </li>
    {% endfor %}
  </ul>
</div>

<style>
  .organizers {
    text-align: center;
  }
  .organizer-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    list-style-type: none;
    padding: 0;
  }
  .organizer-item {
    flex: 1 1 calc(20% - 40px); /* Adjust the size as needed */
    text-align: center;
  }
  .organizer-img {
    width: 150px; /* Adjust the width as needed */
    height: auto; /* Maintain aspect ratio */
    border-radius: 50%; /* Optional: make images circular */
  }
  .organizer-name {
    font-size: 1.0em; /* Adjust the font size as needed */
  }
  .organizer-affiliation {
    font-size: 1.0em; /* Adjust the font size as needed */
  }
</style>

## Sponsors

<div class="sponsors">
  <ul class="sponsor-list">
    {% for sponsor in page.sponsors %}
      <li class="sponsor-item">
        <a href="{{ sponsor.url }}">
          <img src="{{ sponsor.image_path }}" alt="{{ sponsor.alt }}" title="{{ sponsor.title }}" class="sponsor-img">
        </a>
        <p>{{ sponsor.title }}</p>
      </li>
    {% endfor %}
  </ul>
</div>

<style>
  .sponsors {
    text-align: left;
  }
  .sponsor-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    list-style-type: none;
    padding: 0;
  }
  .sponsor-item {
    flex: 1 1 100px; /* Adjust the size as needed */
    text-align: center;
  }
  .sponsor-img {
    width: 200px; /* Set a fixed width */
    height: 100px; /* Set a fixed height */
    object-fit: contain; /* Ensure the image fits within the area without distortion */
  }
</style>

## Contact

If you have any questions, please contact us.

Mail: art-of-robustness-iros2025 [at] googlegroups.com
