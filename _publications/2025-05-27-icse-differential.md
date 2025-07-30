---
collection: publications
downloads:
  paper: /assets/files/publications/ICSE25-Differential.pdf
  artifact: https://github.com/less-lab-uva/DiffTest4AV
  slides: /assets/files/slides/ICSE25-Differential-Slides.pdf
type: inproceedings
author: [Trey Woodlief, Carl Hildebrandt, Sebastian Elbaum]
title: "A Differential Testing Framework to Identify Critical AV Failures Leveraging Arbitrary Inputs"
venue: "International Conference on Software Engineering (ICSE)"
booktitle: "2025 IEEE/ACM International Conference on Software Engineering (ICSE)"
year: 2025
abstract: "The proliferation of autonomous vehicles (AVs) has made their failures increasingly evident. Testing efforts aimed at identifying the inputs leading to those failures are challenged by the input’s long-tail distribution, whose area under the curve is dominated by rare scenarios. We hypothesize that leveraging emerging open-access datasets can accelerate the exploration of long-tail inputs. Having access to diverse inputs, however, is not sufficient to expose failures; an effective test also requires an oracle to distinguish between correct and incorrect behaviors. Current datasets lack such oracles and developing them is notoriously difficult. In response, we propose DIFFTEST4AV, a differential testing framework designed to address the unique challenges of testing AV systems: 1) for any given input, many outputs may be considered acceptable, 2) the long-tail contains an insurmountable number of inputs to explore, and 3) the AV’s continuous execution loop requires for failures to persist in order to affect the system. DIFFTEST4AV integrates statistical analysis to identify meaningful behavioral variations, judges their importance in terms of the severity of these differences, and incorporates sequential analysis to detect persistent errors indicative of potential system-level failures. Our study on 5 versions of the commercially-available, road-deployed comma.ai OpenPilot system, using 3 available image datasets, demonstrates the capabilities of the framework to detect high-severity, high-confidence, long-running test failures."
date: 2025-05-27
---
