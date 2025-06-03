---
title: "Projects"
permalink: /projects/
layout: default
---
  <section class="projects-grid">
  
  <!-- Project Card 1 -->
  <div class="project-card">
    <img src="/assets/images/placeholder.png" alt="Boids GPU Simulation">
    <h3>Boids Simulation with GPU Acceleration</h3>
    <p>Flocking behavior implemented in CUDA and compared with CPU baseline.</p>
    <a href="https://github.com/grastagg/HPC_final_project" class="btn">GitHub Repo</a>
    <button class="modal-btn" data-modal="modal-boids">More Info</button>
  </div>

  <!-- Project Card 2 -->
  <div class="project-card">
    <img src="/assets/images/placeholder.png" alt="Speed Estimation">
    <h3>Monocular Speed Estimation</h3>
    <p>Vehicle speed estimation from a single camera feed.</p>
    <a href="https://github.com/backflipsciboy/SpeedTrap" class="btn">GitHub Repo</a>
    <button class="modal-btn" data-modal="modal-speed">More Info</button>
  </div>

  <!-- Add additional cards here -->

</section>

<!-- Modal Content (placeholders) -->
<div id="modal-boids" class="modal">
  <div class="modal-content">
    <span class="close" data-modal="modal-boids">&times;</span>
    <h2>Boids Simulation with GPU Acceleration</h2>
    <p>README summary extracted from the repository describing the CUDA implementation of the classic boids algorithm...</p>
  </div>
</div>

<div id="modal-speed" class="modal">
  <div class="modal-content">
    <span class="close" data-modal="modal-speed">&times;</span>
    <h2>Monocular Speed Estimation</h2>
    <p>README summary explaining the pipeline for estimating vehicle speeds using computer vision techniques and calibration data...</p>
  </div>
</div>

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
  text-align: center;
  background: white;
}
.project-card img {
  max-width: 100%;
  border-radius: 0.5rem;
}
.btn {
  display: inline-block;
  margin-top: 0.5rem;
  padding: 0.4rem 0.8rem;
  background: #007acc;
  color: white;
  border-radius: 0.5rem;
  text-decoration: none;
}
.modal {
  display: none;
  position: fixed;
  z-index: 999;
  left: 0; top: 0;
  width: 100%; height: 100%;
  background-color: rgba(0,0,0,0.6);
}
.modal-content {
  background-color: #fff;
  margin: 10% auto;
  padding: 2rem;
  width: 90%; max-width: 600px;
  border-radius: 1rem;
}
.close {
  float: right;
  font-size: 1.5rem;
  cursor: pointer;
}
</style>

<script>
document.querySelectorAll('.modal-btn').forEach(btn => {
  btn.onclick = () => {
    const id = btn.getAttribute('data-modal');
    document.getElementById(id).style.display = 'block';
  };
});
document.querySelectorAll('.close').forEach(span => {
  span.onclick = () => {
    const id = span.getAttribute('data-modal');
    document.getElementById(id).style.display = 'none';
  };
});
window.onclick = function(event) {
  if (event.target.classList.contains('modal')) {
    event.target.style.display = 'none';
  }
};
</script>

