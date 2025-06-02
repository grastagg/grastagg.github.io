---
title: "Cooperative Path Planning for UAVs in Contested Environments"
permalink: /research/radar/
layout: single
author_profile: true
---

## Summary

This paper presents cooperative path planning strategies for teams of heterogeneous UAVs operating in radar-threatened environments. The goal is to enable **low-priority sacrificial agents** to explore an area with enemy radar. They are tasked with localizing radar, reducing uncertainty in radar locations and parameters, and exploring. High-priority agent then use this information to plan safe paths through the uncertain radar. We use a linear sensitivity analysis to account for uncertainty in radar probability of detection (PD). We then present two high-priority path planning algorithms--one for the deterministic case where radar parameters are known, and another for the case where radar parameters are uncertain (from the uncertain estimates). 
Key contributions:

 **Cooperative Path Planning for Low-Priority Agents:**  
  We develop an algorithm that optimally balances regional exploration and the reduction of uncertainty in detected radar locations.
- **Path Planning with Known Radar Parameters:**  
  Utilizing weighted Voronoi diagrams, we design a path planning algorithm that minimizes radar detection risk when radar parameters are fully known.
- **Path Planning with Uncertain Radar Parameters:**  
  For scenarios with uncertain radar parameters, we introduce a path planning algorithm based on generalized Voronoi diagrams to enhance the stealth and survivability of a high-value UAV.

---

## Figure

![Cooperative radar inference and path planning](/assets/images/radar-overview.png)

*Figure: Coordination of low-priority (exploratory) and high-priority (protected) UAVs navigating through a radar field.*

---


## Abstract

In contested environments, UAVs often encounter threats from adversarial sensors such as ground-based radar. Planning safe paths through such environments requires knowledge of the location and coverage of radar fields, which is often unavailable or uncertain. This work proposes a cooperative multi-agent framework for planning in such settings.

Low-priority agents are tasked with exploring the environment and intentionally entering suspected radar zones to gather data on the adversary’s location and capabilities. High-priority agents use this data to avoid radar fields. We introduce a novel risk-aware planning algorithm that combines Bayesian inference, radar detection models, and Voronoi-based path planning to coordinate agents of different priority levels.

Simulation results demonstrate that this cooperative strategy significantly improves mission success rates for high-priority agents while maintaining acceptable losses for exploratory agents.

---

## Citation

G. Stagg and C. K. Peterson,  
**“Cooperative Multi-Agent Path Planning for Heterogeneous UAVs in Contested Environments”**  
*In preparation for submission.*  
[PDF](/assets/files/radar-paper.pdf)

