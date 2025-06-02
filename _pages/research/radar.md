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

![Low-Priority Path Planning](/assets/images/lpp_objective.png)

*Figure: The three different parts of the objective function. The left figure shows the covariance reduction objective function. The
estimated radar location is plotted in red. From this figure we see that the best measurement locations to reduce a radar’s uncertainty (covariance of the EKF) come from being closer to the radar, and from going perpendicular to the current measurements. The middle figure illustrates the
exploration objective function, where the green points show locations the agents have already explored. Going further from the explored area provides
better measurements. The final plot shows the distance to goal objective, where the goal is in the upper right corner of the plot.*

---

![High-Priority Path Planning Known Radar Parameters](/assets/images/det_hpp.png)

*Figure: This figure shows the steps of our deterministic high-priority path planning algorithm. In the top left figure, the weighted Voronoi
diagram is found. Then all edges where the PD is above a threshold for any point along the edge are removed. In the top right figure, A-star is used to find the shortest path
through the graph. In the bottom left, a B-spline is fit to the A-star path. Then, in the bottom center, the optimized B-spline is shown. All figures show the
locations of the radar as red x’s with the PD at every location depicted by the heatmap.*

---

![High-Priority Path Planning Uncertain Radar Parameters](/assets/images/uncertain_hpp.png)

*Figure: his figure shows the steps of our uncertain high-priority path planning algorithm. In the top left figure, the generalized Voronoi diagram
is found using the probability the PD is below the threshold as the metric. Then all edges where the probability the PD is below a threshold is less than a safety parameter are removed. In the top right figure, A-star is used to find the
shortest path through the graph. In the bottom left, a B-spline is fit to the A-star path. Then, in the bottom center, the optimized B-spline is shown. Finally,
the bottom left image shows the path safety metric. In this figure, the low-priority agents’ paths are shown in red. All figures show the current estimated
location of the radar as red x’s. The first five show the probability the PD is below the threshold as the heatmap*

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

