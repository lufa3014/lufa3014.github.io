---
permalink: /projects/
title: "Projects"
---

<div>
  <h2>
    G.R.I.D. – Strategy/Tactics Game in Unity
    <a href="https://github.com/lufa3014/Grid-Prototyp.git" style="margin-left: 10px;">
      <img src="https://img.shields.io/badge/GitHub-View%20Repository-blue?logo=github" alt="GitHub Repo" style="vertical-align: middle;">
    </a>
  </h2>
  <p>
    <strong>Module:</strong> Game Design Project<br>
    <strong>Role:</strong> Game Designer &amp; Developer (2-person team)<br>
    <strong>Period:</strong> 04/2024 – 03/2025
  </p>
  <p>
    Conceptualization and development of a 3D single-player game in Unity with a focus on game balance, visual clarity, and technical extensibility. Responsible for core gameplay systems, deckbuilding logic, CI/CD pipeline, and project-specific tools.
  </p>
  <div id="grid-gallery" style="text-align:center;">
    <img id="grid-image" src="/assets/images/GRID-Battle.png" alt="GRID Battle" style="max-width: 100%; border-radius: 4px;">
  </div>
</div>

<script>
  const images = [
    "/assets/images/GRID-Battle.png",
    "/assets/images/GRID-Closeup.png",
    "/assets/images/GRID-Deckbuilder.png"
  ];
  let current = 0;
  function showImage(idx) {
    document.getElementById('grid-image').src = images[idx];
  }
  setInterval(() => {
    current = (current + 1) % images.length;
    showImage(current);
  }, 4500);
</script>

<div style="margin-top:40px;">
  <h2>
    Level Design – Chamber & Cave
  </h2>
  <p>
    <strong>Module:</strong> Level Design<br>
    <strong>Role:</strong> Level Designer<br>
    <strong>Period:</strong> 2024
  </p>
  <p>
    Creation and visualization of game levels with a focus on spatial composition, player guidance, and atmosphere. Animated GIFs show two different level prototypes: Chamber and Cave.
  </p>
  <div style="display: flex; gap: 32px; justify-content: center;">
    <img src="/assets/images/LEVEL_DESIGN-CHAMBER.gif" alt="Level Design Chamber" style="max-width: 350px; border-radius: 12px;">
    <img src="/assets/images/LEVEL-DESIGN-CAVE.gif" alt="Level Design Cave" style="max-width: 350px; border-radius: 12px;">
  </div>
</div>