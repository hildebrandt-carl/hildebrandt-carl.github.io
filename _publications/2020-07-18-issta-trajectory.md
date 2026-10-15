---
collection: publications
downloads:
  paper: /assets/files/publications/ISSTA20-Trajectory.pdf
  artifact: https://github.com/hildebrandt-carl/RobotTestGeneration
  video: https://www.youtube.com/watch?v=CGzUuVX2b3k
  slides: /assets/files/slides/ISSTA20-Trajectory-Slides.pdf
type: inproceedings
author: [Carl Hildebrandt, Sebastian Elbaum, Nicola Bezzo, Matthew B. Dwyer]
title: "Feasible and Stressful Trajectory Generation for Mobile Robots"
venue: "International Symposium on Software Testing and Analysis (ISSTA)"
booktitle: "Proceedings of the 29th ACM SIGSOFT International Symposium on Software Testing and Analysis (ISSTA)"
pages: "349-362"
year: 2020
access_url: https://dl.acm.org/doi/10.1145/3395363.3397387
doi: 10.1145/3395363.3397387
abstract: "While executing nominal tests on mobile robots is required for their validation, such tests may overlook faults that arise under trajectories that accentuate certain aspects of the robot's behavior. Uncovering such stressful trajectories is challenging as the input space for these systems, as they move, is extremely large, and the relation between a planned trajectory and its potential to induce stress can be subtle. To address this challenge we propose a framework that 1) integrates kinematic and dynamic physical models of the robot into the automated trajectory generation in order to generate valid trajectories, and 2) incorporates a parameterizable scoring model to efficiently generate physically valid yet stressful trajectories for a broad range of mobile robots. We evaluate our approach on four variants of a state-of-the-art quadrotor in a racing simulator. We find that, for non-trivial length trajectories, the incorporation of the kinematic and dynamic model is crucial to generate any valid trajectory, and that the approach with the best hand-crafted scoring model and with a trained scoring model can cause on average a 55.9% and 41.3% more stress than a random selection among valid trajectories. A follow-up study shows that the approach was able to induce similar stress on a deployed commercial quadrotor, with trajectories that deviated up to 6m from the intended ones."
citation: "Carl Hildebrandt, Sebastian Elbaum, Nicola Bezzo, Matthew B. Dwyer. 2020. Feasible and Stressful Trajectory Generation for Mobile Robots. In <i>Proceedings of the 29th ACM SIGSOFT International Symposium on Software Testing and Analysis. (ISSTA)</i>. 349-362. https://doi.org/10.1145/3395363.3397387"
date: 2020-07-18
---


