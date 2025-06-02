---
title: "Cooperative Path Planning for UAVs in Contested Environments"
permalink: /research/radar/
layout: single
author_profile: true
---

## Summary

This paper presents cooperative path planning strategies for teams of heterogeneous UAVs operating in radar-threatened environments. The goal is to enable **low-priority sacrificial agents** to explore an area with enemy radar. They are tasked with localizing radar, reducing uncertainty in radar locations and parameters, and exploring. High-priority agent then use this information to plan safe paths through the uncertain radar. We use a linear sensitivity analysis to account for uncertainty in radar probability of detection (PD). We then present two high-priority path planning algorithms--one for the deterministic case where radar parameters are known, and another for the case where radar parameters are uncertain (from the uncertain estimates). 
Key contributions:
 - **Cooperative Path Planning for Low-Priority Agents:**  
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
This paper addresses the challenge of navigating
unmanned aerial vehicles (UAV) in contested environments by
introducing a cooperative multi-agent framework that increases
the likelihood of safe UAV traversal. The approach involves two
types of UAVs: low-priority agents that explore and localize
threats, and a high-priority agent that navigates safely to its
target destination while minimizing the risk of detection by
enemy radar systems. The low-priority agents employ a decen-
tralized optimization algorithm to balance exploration, radar
localization, and safe path identification for the high-priority
agent. For the high-priority agent, two path-planning methods
are proposed: one for deterministic scenarios using weighted
Voronoi diagrams, and another for uncertain scenarios leveraging
generalized Voronoi diagrams and probabilistic constraints. Both
methods employ optimization techniques to refine the trajec-
tories while accounting for kinematic constraints and radar
detection probabilities. Numerical simulations demonstrate the
effectiveness of our framework. This research advances UAV path
planning methodologies by combining heterogeneous multi-agent
cooperation, probabilistic modeling, and optimization to enhance
mission success in adversarial environments.

---

## Citation

G. Stagg and C. K. Peterson,  
**“Cooperative Multi-Agent Path Planning for Heterogeneous UAVs in Contested Environments”**  
*In preparation for submission.*  
[PDF](/assets/files/radar-paper.pdf)

