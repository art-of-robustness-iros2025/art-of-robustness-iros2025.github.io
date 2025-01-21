---
permalink: /
layout: splash

sponsors:
  - url: https://eng.bigai.ai/
    image_path: /assets/images/sponsors/BIGAI.png
    alt: "BIGAI"

invited_speakers:
  - name: "Prof. XXX"
    affiliation: "University of XXX"
    image_path: /assets/images/invited_speakers/bio-photo.jpg
    topic: "Title of the Talk"

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
  - name: "Russell Buchanan"
    affiliation: "University of Waterloo"
    image_path: /assets/images/organizers/russell.jpeg
  - name: Yue Gao
    affiliation: "Shanghai Jiaotong University"
    image_path: /assets/images/organizers/yue.jpeg
  - name: Hangxin Liu
    affiliation: "Beijing Institute for General Artificial Intelligence (BIGAI)"
    image_path: /assets/images/organizers/hangxin.jpg
  - name: Yao Su
    affiliation: "Beijing Institute for General Artificial Intelligence (BIGAI)"
    image_path: /assets/images/organizers/yao.jpeg
---

**Warning Notice:** This website is under construction.
{: .notice--warning}

# The Art of Robustness: Surviving Failures in Robotics @ IROS 2025

*October 20, 2025 in Hangzhou, China*

## Abstract

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
robustness of robotic systems**. The workshop will bring together world-renowned researchers and practitioners
from diverse fields, including whole-body model-based control, robot learning, perception and sensing, to share
their insights and experiences. The workshop will feature invited talks, poster sessions, and panel discussions,
offering attendees a comprehensive understanding on robustness challenges in robotics and highlight the latest
advancements and strategies for addressing these obstacles.

## Topics of Dicussion and Interest

The workshop will focus on the following topics:

- Analyzing the key challenges that lead to failures in robotics, namely perceptual noise, uncertainty in model-based methods, limited generalizability in learning-based methods. 

- Exploring innovative solutions to mitigate these issues, thereby improving the robustness of robotic systems. 

- System integration


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
  </style>

## Call for Posters

We invite researchers to submit short papers on preliminary results, ongoing works, and demos relevant to the workshop to _Link_ in the form of a short papers (2-4 pages, excluding references).

**Important Dates**

**First Round Submission**
- **Submission Deadline**: 5th August 2025
- **Notification**: 20th August 2025

**Second Round Submission**
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
    text-align: center;
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
    width: 250px; /* Adjust the width as needed */
    height: auto; /* Maintain aspect ratio */
  }
</style>

## Contact

If you have any questions, please contact us.

Mail: iros2025_robust_robot_ws [at] googlegroups.com