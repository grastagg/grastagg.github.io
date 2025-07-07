---
title: "Projects"
permalink: /projects/
layout: single
author_profile: true
---

<style>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
  padding: 1rem 0;
}
.project-tile {
  background: #fff;
  border-radius: 1rem;
  overflow: hidden;
  border: 1px solid #ddd;
  padding: 1rem;
  display: flex;
  flex-direction: column;
  transition: box-shadow 0.3s ease;
}
.project-tile:hover {
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}
.project-tile img,
.project-tile video {
  width: 100%;
  height: auto;
  margin-bottom: 0.75rem;
  border-radius: 0.5rem;
}
.project-tile h3 {
  margin: 0.25rem 0;
}
.project-tile p {
  font-size: 0.95rem;
  color: #333;
  flex-grow: 1;
}
.project-tile a {
  color: #007acc;
  text-decoration: none;
  margin-top: 0.5rem;
  font-weight: bold;
  display: inline-block;
}
.featured-carousel {
  overflow-x: auto;
  overflow-y: hidden;
  padding: 1rem 0;
  margin-bottom: 2rem;
}
.carousel-track {
  display: flex;
  gap: 1.5rem;
  scroll-snap-type: x mandatory;
}
.carousel-card {
  min-width: 300px;
  flex: 0 0 auto;
  background: #fff;
  border-radius: 1rem;
  border: 1px solid #ddd;
  padding: 1rem;
  scroll-snap-align: start;
  box-shadow: 0 2px 6px rgba(0,0,0,0.05);
}
.carousel-card video,
.carousel-card img {
  width: 100%;
  height: auto;
  border-radius: 0.5rem;
  margin-bottom: 0.75rem;
}
.carousel-card h3 {
  margin: 0.5rem 0 0.25rem;
}
.carousel-card p {
  font-size: 0.9rem;
  color: #333;
}
.carousel-card a {
  color: #007acc;
  font-weight: bold;
  text-decoration: none;
  margin-top: 0.5rem;
  display: inline-block;
}
</style>
## Featured Projects

<div class="featured-carousel">
  <div class="carousel-track">

    <div class="carousel-card">
      <video autoplay loop muted playsinline>
        <source src="/assets/videos/fpv-sim.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <h3>FPV Drone Simulator</h3>
      <p>C++ + OpenSceneGraph drone simulation with quad dynamics and controller input.</p>
      <a href="https://github.com/grastagg/fpv_drone_sim.git">GitHub</a>
    </div>

    <div class="carousel-card">
      <video autoplay loop muted playsinline>
        <source src="/assets/videos/rl_car.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <h3>RL RC Car Driver</h3>
      <p>Reinforcement learning to control an RC car from raw camera input.</p>
      <a href="https://github.com/grastagg/SelfDrivingCarClassTeam4">GitHub</a>
    </div>

    <div class="carousel-card">
      <img src="/assets/videos/rl_drone.gif" alt="RL Drone">
      <h3>RL Target Acquisition</h3>
      <p>RL agent learns to track targets while avoiding dynamic obstacles.</p>
      <a href="https://github.com/ajordan5/RL-Target-Acquisition">GitHub</a>
    </div>

    <div class="carousel-card">
      <video autoplay loop muted playsinline>
        <source src="/assets/videos/ants.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
      <h3>Ant Colony Simulation</h3>
      <p>Local sensing, pheromone trails, and coordinated food gathering in C++.</p>
      <a href="https://github.com/grastagg/ant_colonoy_simulation.git">GitHub</a>
    </div>

  </div>
</div>


<section class="projects-grid">

  <div class="project-tile">
    <img src="/assets/videos/rl_drone.gif" alt="RL Target Acquisition">
    <h3>RL Target Acquisition and Obstacle Avoidance</h3>
    <p>Used reinforcement learning to control an agent for locating targets while avoiding dynamic obstacles in a simulated environment. The project poster is available <a href="/assets/files/TargetAcquisition.pdf">here</a>.</p>
    <a href="https://github.com/ajordan5/RL-Target-Acquisition">GitHub</a>
  </div>

  <div class="project-tile">
    <video autoplay loop muted playsinline>
      <source src="/assets/videos/rl_car.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <h3>RL-Based RC Car Driver</h3>
    <p>Trained an RC car to follow a track using reinforcement learning with camera input.</p>
    <a href="https://github.com/grastagg/SelfDrivingCarClassTeam4">GitHub</a>
  </div>

  <div class="project-tile">
    <video autoplay loop muted playsinline>
      <source src="/assets/videos/fpv-sim.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <h3>FPV Drone Simulator</h3>
    <p>Drone simulator built using OpenSceneGraph and C++ with physical quadcopter modeling and controller input support.</p>
    <a href="https://github.com/grastagg/fpv_drone_sim.git">GitHub</a>
  </div>

  <div class="project-tile">
    <video autoplay loop muted playsinline>
      <source src="/assets/videos/ants.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    <h3>Ant Colony Simulation</h3>
    <p>C++ simulation where ants follow pheromone trails to locate and share food sources. Includes local sensing, trail decay, and group coordination.</p>
    <a href="https://github.com/grastagg/ant_colonoy_simulation.git">GitHub</a>
  </div>

  <div class="project-tile">
    <img src="/assets/images/hallway-car.gif" alt="ECENRacer">
    <h3>Self-Driving Car with Segmentation</h3>
    <p>Steered a car through hallways using a segmentation network to identify walls and floor regions.</p>
    <a href="https://github.com/backflipsciboy/ECENRacer">GitHub</a>
  </div>

  <div class="project-tile">
    <img src="/assets/images/baseball-catcher.gif" alt="Baseball Catcher">
    <h3>Baseball Catcher</h3>
    <p>Used stereo vision and kinematics to predict a baseball’s landing location and actuate a net to catch it.</p>
    <a href="https://github.com/backflipsciboy/BaseballCatcher">GitHub</a>
  </div>

  <div class="project-tile">
    <img src="/assets/images/boids.gif" alt="Boids Simulation">
    <h3>GPU-Accelerated Boids Simulation</h3>
    <p>Simulated flocking behavior on both CPU and GPU using CUDA for parallel speedups.</p>
    <a href="https://github.com/grastagg/HPC_final_project">GitHub</a>
  </div>

  <div class="project-tile">
    <img src="/assets/images/speed-estimation.gif" alt="Speed Estimation">
    <h3>Monocular Speed Estimation</h3>
    <p>Estimated the speed of vehicles using only a single calibrated camera input.</p>
    <a href="https://github.com/backflipsciboy/SpeedTrap">GitHub</a>
  </div>

  <div class="project-tile">
    <img src="/assets/images/uav-landing.gif" alt="Landing Trajectory">
    <h3>UAV Landing Trajectory Generator</h3>
    <p>Generated landing paths using B-splines and differential flatness-based optimization.</p>
  </div>

  <div class="project-tile">
    <img src="/assets/images/gpr-estimation.gif" alt="GPR Estimator">
    <h3>Continuous-Time Batch State Estimation with GPR</h3>
    <p>Used Gaussian Process Regression to estimate smooth continuous-time trajectories from noisy measurements.</p>
  </div>

  <div class="project-tile">
    <img src="/assets/images/icp.gif" alt="2D ICP Lidar">
    <h3>2D ICP for Lidar Scan Matching</h3>
    <p>Implemented the Iterative Closest Point algorithm for aligning sequential 2D lidar scans and improving pose estimation.</p>
  </div>

</section>
