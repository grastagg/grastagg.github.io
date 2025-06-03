---
title: "Projects"
permalink: /projects/
layout: default
---

<style>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}
.project-card {
  border: 1px solid #ccc;
  padding: 1rem;
  border-radius: 1rem;
  text-align: left;
  background: white;
  transition: box-shadow 0.3s;
}
.project-card:hover {
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}
.project-card img {
  max-width: 100%;
  border-radius: 0.5rem;
  margin-bottom: 0.75rem;
}
.project-description {
  display: none;
  margin-top: 0.5rem;
  font-size: 0.95rem;
  color: #333;
}
.project-card button {
  background: none;
  color: #007acc;
  border: none;
  padding: 0;
  cursor: pointer;
  font-size: 0.9rem;
  margin-top: 0.5rem;
  text-decoration: underline;
}
</style>

<section class="projects-grid">
  
  <!-- Project 1 -->
  <div class="project-card">
    <img src="/assets/images/placeholder.png" alt="Boids GPU Simulation">
    <h3>Boids Simulation with GPU Acceleration</h3>
    <p>Flocking behavior implemented using CUDA and CPU baselines.</p>
    <a href="https://github.com/grastagg/HPC_final_project" class="btn">GitHub Repo</a>
    <button onclick="toggleDescription(this)">More Info</button>
    <div class="project-description">
      Implementation of the classical Boids algorithm in parallel using both GPU and CPU, optimizing performance across different architectures.
    </div>
  </div>

  <!-- Project 2 -->
  <div class="project-card">
    <img src="/assets/images/placeholder.png" alt="Speed Estimation">
    <h3>Monocular Speed Estimation</h3>
    <p>Estimates vehicle speed from a single video stream.</p>
    <a href="https://github.com/backflipsciboy/SpeedTrap" class="btn">GitHub Repo</a>
    <button onclick="toggleDescription(this)">More Info</button>
    <div class="project-description">
      Uses monocular vision and calibration techniques to approximate vehicle speeds in real-time.
    </div>
  </div>

  <!-- Add more projects here following the same format -->

</section>

<script>
function toggleDescription(button) {
  const desc = button.nextElementSibling;
  if (desc.style.display === "block") {
    desc.style.display = "none";
    button.textContent = "More Info";
  } else {
    desc.style.display = "block";
    button.textContent = "Less Info";
  }
}
</script>

