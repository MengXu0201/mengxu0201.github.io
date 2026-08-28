---
layout: archive
title: "Photo Gallery"
permalink: /gallery/
author_profile: true
---

{% include base_path %}

<style>
  .gallery-event {
    margin-top: 2.5em;
  }

  .gallery-event:first-of-type {
    margin-top: 0;
  }

  .gallery-event h2 {
    margin-top: 0;
    margin-bottom: 0.35em;
  }

  .gallery-description {
    margin-top: 0;
    margin-bottom: 1em;
  }

  .gallery-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1em;
    align-items: start;
  }

  .gallery-grid img,
  .gallery-single img {
    display: block;
    width: 100%;
    height: auto;
  }

  .gallery-single {
    max-width: 700px;
    margin-left: auto;
    margin-right: auto;
  }

  @media (max-width: 600px) {
    .gallery-grid {
      grid-template-columns: 1fr;
    }
  }
</style>

<section class="gallery-event">
  <h2>Commencement 2026</h2>
  <p class="gallery-description">Celebrating the 2026 commencement with students from the Department of Computer Science and Technology.</p>
  <div class="gallery-grid">
    <img src="{{ '/images/gallery/ceremony_graduate_students_2026.jpg' | relative_url }}" alt="Commencement 2026 with graduate students">
    <img src="{{ '/images/gallery/ceremony_students_2026.JPG' | relative_url }}" alt="Commencement 2026 with students">
    <img src="{{ '/images/gallery/ceremony_rayleen_2026.JPG' | relative_url }}" alt="Commencement 2026 with Rayleen Ramos">
    <img src="{{ '/images/gallery/ceremony_cesar_2026.JPG' | relative_url }}" alt="Commencement 2026 with Cesar Marte Jimenez">
  </div>
</section>

<section class="gallery-event">
  <h2>Commencement 2025</h2>
  <p class="gallery-description">Celebrating the 2025 commencement with faculty and students from the Department of Computer Science and Technology.</p>
  <div class="gallery-grid">
    <img src="{{ '/images/gallery/ceremony_colleage_2025.JPEG' | relative_url }}" alt="Commencement 2025 with faculty">
    <img src="{{ '/images/gallery/ceremony_students_2025.JPG' | relative_url }}" alt="Commencement 2025 with students">
  </div>
</section>

<section class="gallery-event">
  <h2>International Symposium on Biomedical Imaging (ISBI) 2025</h2>
  <p class="gallery-description">Presenting our work at ISBI 2025 in Houston.</p>
  <div class="gallery-grid">
    <img src="{{ '/images/gallery/ISBI_Houston_me.JPG' | relative_url }}" alt="ISBI 2025 in Houston">
    <img src="{{ '/images/gallery/ISBI_Houston_kuan.JPG' | relative_url }}" alt="ISBI 2025 in Houston">
  </div>
</section>

<section class="gallery-event">
  <h2>Senior Research Presentation 2025</h2>
  <p class="gallery-description">With students presenting their supervised senior research projects in 2025.</p>
  <div class="gallery-single">
    <img src="{{ '/images/gallery/Senior_research_presentation_2025.JPG' | relative_url }}" alt="Senior Research Presentation 2025">
  </div>
</section>

<section class="gallery-event">
  <h2>Commencement 2024</h2>
  <p class="gallery-description">Celebrating the 2024 commencement with faculty and students from the Department of Computer Science and Technology.</p>
  <div class="gallery-grid">
    <img src="{{ '/images/gallery/ceremony_colleage_2024.JPG' | relative_url }}" alt="Commencement 2024 with faculty">
    <img src="{{ '/images/gallery/ceremony_students_2024.jpg' | relative_url }}" alt="Commencement 2024 with students">
  </div>
</section>
