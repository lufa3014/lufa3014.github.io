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
    Sneaky - Stealth/Puzzle Game in Unity
    <a href="https://github.com/lufa3014/Level-Design.git" style="margin-left: 10px;">
      <img src="https://img.shields.io/badge/GitHub-View%20Repository-blue?logo=github" alt="GitHub Repo" style="vertical-align: middle;">
    </a>
  </h2>
  <p>
    <strong>Module:</strong> Level Design<br>
    <strong>Role:</strong> Level Designer (2-person team)<br>
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
    EntityEvents – Lightweight Event System for Unity ECS
    <a href="https://github.com/lufa3014/EntityEvents.git" style="margin-left: 10px;">
      <img src="https://img.shields.io/badge/GitHub-View%20Repository-blue?logo=github" alt="GitHub Repo" style="vertical-align: middle;">
    </a>
  </h2>
  <p>
    <strong>Type:</strong> Personal Project<br>
    <strong>Role:</strong> Developer<br>
    <strong>Period:</strong> 2025
  </p>
  <p>
    A lightweight, modular event system for Unity ECS, using Roslyn source generators for fast and type-safe event handling. Features include custom event types, event buffers, and automatic conversion between buffer elements and events. Designed for scalable, decoupled gameplay logic in DOTS projects.
  </p>
  <p><strong>Example usage:</strong></p>

  <details>
    <summary>Show code example</summary>
    
    ````csharp
    // Define an event
    [Event(WorldSystemFilterFlags.Default)]
    public struct DamageEvent : IComponentData
    {
        public int Amount;
    }

    // Convert buffer element to event
    public struct DamageEventBuffer : IBufferElementData, IEventConverter<DamageEvent>
    {
        public int Amount;
        public DamageEvent ToEvent() => new DamageEvent { Amount = Amount };
    }

    // Usage in system
    public partial struct DamageEventManager : ISystem
    {
        public void OnUpdate(ref SystemState state)
        {
            new EventManager<DamageEvent, DamageEventBuffer>().OnUpdate(ref state);
        }
    }
    ````
</details>
</div>