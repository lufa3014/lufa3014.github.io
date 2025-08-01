---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: single
author_profile: true
permalink: /
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
    VR Cooking Game – Physics-Based VR Experience in Unity
  </h2>
  <p>
    <strong>Module:</strong> VR Project<br>
    <strong>Role:</strong> Technical Lead (4-person team)<br>
    <strong>Period:</strong> 01/2025 – 06/2025
  </p>
  <p>
    Physics-based VR game in Unity featuring interaction systems for ingredients, cooking processes, and customers. Developed the game loop, timer system, event system, VR-specific systems, and audio integration.
  </p>
  <div style="text-align:center;">
    <video controls style="max-width: 100%; border-radius: 12px;">
      <source src="/assets/videos/VR-Trailer.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

<div style="margin-top:40px;">
  <h2>
    Sneaky - Stealth/Puzzle Game in Unity
    <a href="https://github.com/lufa3014/Level-Design.git" style="margin-left: 10px;">
      <img src="https://img.shields.io/badge/GitHub-View%20Repository-blue?logo=github" alt="GitHub Repo" style="vertical-align: middle;">
    </a>
  </h2>
  <p>
    <strong>Module:</strong> Level Design<br>
    <strong>Role:</strong> Game Designer &amp; Developer (2-person team)<br>
    <strong>Period:</strong> 04/2023 – 06/2023
  </p>
  <p>
    Development of a 3D puzzle/stealth game in Unity with a focus on level design. Responsible for enemy AI, animation systems, interactive objects, chat window, and shader effects.
  </p>
  <div id="level-gallery" style="text-align:center;">
    <img id="level-image" src="/assets/images/LEVEL_DESIGN-CHAMBER.gif" alt="Level Design Chamber" style="max-width: 100%; border-radius: 12px;">
  </div>
</div>

<script>
  const levelImages = [
    "/assets/images/LEVEL_DESIGN-CHAMBER.gif",
    "/assets/images/LEVEL-DESIGN-CAVE.gif"
  ];
  let levelCurrent = 0;
  function showLevelImage(idx) {
    document.getElementById('level-image').src = levelImages[idx];
  }
  setInterval(() => {
    levelCurrent = (levelCurrent + 1) % levelImages.length;
    showLevelImage(levelCurrent);
  }, 14500);
</script>

<div style="margin-top:40px;">
  <h2>
    Rendering Engine in OpenGL & C
    <a href="https://github.com/lufa3014/Deferred-Rendering-Engine.git" style="margin-left: 10px;">
      <img src="https://img.shields.io/badge/GitHub-View%20Repository-blue?logo=github" alt="GitHub Repo" style="vertical-align: middle;">
    </a>
  </h2>
  <p>
    <strong>Module:</strong> Visual Effects & Shader<br>
    <strong>Role:</strong> Developer (2-person team)<br>
    <strong>Period:</strong> 10/2024 – 01/2025
  </p>
  <p>
    Development of a 3D engine with deferred rendering, Phong shading, normal mapping, tessellation, shadow mapping, and postprocessing. Implemented camera, lighting, and scene systems, dynamic shader reloading, and GUI integration.
  </p>
  <div id="renderer-gallery" style="text-align:center;">
    <img id="renderer-image" src="/assets/images/Renderer-NormalMapping.png" alt="Normal Mapping" style="max-width: 100%; border-radius: 12px;">
  </div>
</div>

<script>
  const rendererImages = [
    "/assets/images/Renderer-NormalMapping.png",
    "/assets/images/Renderer-ShadowMapping.png",
    "/assets/images/Renderer-SmallScene.png",
    "/assets/images/RendererDisplacement.png"
  ];
  let rendererCurrent = 0;
  function showRendererImage(idx) {
    document.getElementById('renderer-image').src = rendererImages[idx];
  }
  setInterval(() => {
    rendererCurrent = (rendererCurrent + 1) % rendererImages.length;
    showRendererImage(rendererCurrent);
  }, 4500);
</script>

<div style="margin-top:40px;">
  <h2>
    Grass Renderer in OpenGL & C
    <a href="https://github.com/lufa3014/Grass-Renderer.git" style="margin-left: 10px;">
      <img src="https://img.shields.io/badge/GitHub-View%20Repository-blue?logo=github" alt="GitHub Repo" style="vertical-align: middle;">
    </a>
  </h2>
  <p>
    <strong>Module:</strong> Geometric Modeling & Computer Animation<br>
    <strong>Role:</strong> Developer (2-person team)<br>
    <strong>Period:</strong> 10/2024 – 01/2025
  </p>
  <p>
    Development of a real-time grass renderer in OpenGL & C featuring Phong-lit animated grass, LODs, frustum culling, spline-based terrain generation, and GPU instancing.
  </p>
  <div id="grass-gallery" style="text-align:center;">
    <img id="grass-image" src="/assets/images/Grass.gif" alt="Phong-Lit Grass" style="max-width: 100%; border-radius: 12px;">
  </div>
</div>