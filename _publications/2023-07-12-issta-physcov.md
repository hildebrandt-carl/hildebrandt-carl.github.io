---
collection: publications
downloads:
  paper: /assets/files/publications/ISSTA23-PhysCov.pdf
  artifact: https://github.com/hildebrandt-carl/PhysicalCoverage
  video: https://www.youtube.com/watch?v=NAGcOydSh6s
  slides: /assets/files/slides/ISSTA23-PhysCov-Slides.pdf
type: inproceedings
author: [Carl Hildebrandt, Meriel von Stein, Sebastian Elbaum]
title: "PhysCov: Physical Test Coverage for Autonomous Vehicles"
venue: "International Symposium on Software Testing and Analysis (ISSTA)"
booktitle: "Proceedings of the 32nd ACM SIGSOFT International Symposium on Software Testing and Analysis (ISSTA)"
pages: "449-461"
year: 2023
access_url: https://dl.acm.org/doi/pdf/10.1145/3597926.3598069
doi: 10.1145/3597926.3598069
abstract: "Adequately exercising the behaviors of autonomous vehicles is fundamental to their validation. However, quantifying an autonomous vehicle's testing adequacy is challenging as the system's behavior is influenced both by its state as well as its physical environment.To address this challenge, our work builds on two insights. First, data sensed by an autonomous vehicle provides a unique spatial signature of the physical environment inputs.Second, given the vehicle's current state, inputs residing outside the autonomous vehicle's physically reachable regions are less relevant to its behavior. Building on those insights, we introduce an abstraction that enables the computation of a physical environment-state coverage metric, PhysCov. The abstraction combines the sensor readings with a physical reachability analysis based on the vehicle's state and dynamics to determine the region of the environment that may affect the autonomous vehicle. It then characterizes that region through a parameterizable geometric approximation that can trade quality for cost. Tests with the same characterizations are deemed to have had similar internal states and exposed to similar environments and thus likely to exercise the same set of behaviors, while tests with distinct characterizations will increase PhysCov. A study on two simulated and one real system's dataset examines PhysCovs's ability to quantify an autonomous vehicle's test suite, showcases its characterization cost and precision, investigates its correlation with failures found and potential for test selection, and assesses its ability to distinguish among real-world scenarios."
citation: "Carl Hildebrandt, Meriel von Stein, Sebastian Elbaum. 2023. PhysCov: Physical Test Coverage for Autonomous Vehicles. In <i>Proceedings of the 32nd ACM SIGSOFT International Symposium on Software Testing and Analysis. (ISSTA)</i>. 449-461. https://doi.org/10.1145/3597926.3598069"
date: 2023-07-12
---


