# 360° Multi-Camera Person Tracking & Re-Identification

[← Back to portfolio](../README.md)

**Ongoing undergraduate research · National Chung Cheng University · Industry collaboration with RockCore**  
**Advisor:** Prof. Wei-Yang Lin

## Research problem

In a multi-camera smart-manufacturing environment, the same individual may appear at different positions, angles, scales, and distortions. With 360° panoramic imagery, perspective effects and image stitching further complicate appearance-based matching. The goal is to maintain **consistent global identities** across cameras while evaluating tracking performance rigorously.

## My areas of contribution

- **Pipeline and integration:** explored how person detection, local tracking, ReID embeddings, and cross-camera global-ID association work together.
- **Model comparison:** evaluated OSNet, TransReID, and CLIP-ReID on preliminary self-collected data; observed that favorable baseline scores can reflect an insufficiently challenging evaluation set.
- **Ground truth and evaluation:** prepared annotation material for HOTA-based assessment, focusing on identity continuity rather than detection accuracy alone.
- **Association constraints:** studied one-to-one assignment for simultaneous individuals (including the Hungarian algorithm) and considered temporal/geometric consistency.
- **Experimental exploration:** compared face/body feature fusion offline and considered trade-offs involving accuracy, latency, and reliability.

## Evaluation principles

- Avoid evaluating on near-identical observations from the same scene in both training and testing.
- Report the data collection and split protocol and limitations.
- Evaluate identity association with tracking-aware metrics such as **HOTA**; examine failure cases across viewpoints and camera boundaries.
- Distinguish preliminary exploratory experiments from fully validated conclusions.

## Current status and availability

**This is ongoing collaborative research.** The working repository is private, and no unpublished experiment datasets, source files, or visual assets are released here. This page describes the public-safe problem formulation and workflow; it does not claim a completed publication or benchmark.

For legitimate academic interest or collaboration, please [contact me](mailto:iddw1498@gmail.com). Additional details may depend on the research team's permission.
