# Kidney Microvascular Segmentation with 2D U-Net

**Individual medical image analysis coursework · MATLAB · 2025**

[← Back to portfolio](../README.md)

## Task

This earlier assignment was **different from my later acute-appendicitis CT project**. It explored vessel segmentation in **PAS-stained kidney histology tiles**, inspired by the HuBMAP Hacking the Human Vasculature competition.

The assignment's goal was to identify blood-vessel regions in 10 test TIFF images and export segmentation-related results. The provided teaching subset contained 1,500 training tiles and polygon-annotation JSON files; I selected **289 Dataset 1 tiles** with expert-reviewed annotations for my pipeline.

## Pipeline

1. Read TIFF tiles, metadata and polygon annotations.
2. Convert polygon coordinates to pixel masks using MATLAB `poly2mask`.
3. Generate extra training samples through geometric augmentation.
4. Reduce the segmentation objective to **blood vessel vs. background**.
5. Split the prepared samples **85% for training / 15% for validation**.
6. Implement a 2D U-Net inspired by a teaching example, including encoder/decoder stages.
7. Address class imbalance by switching from an ordinary pixel-classification output to a **Dice-based loss**.
8. Train the model and visualize predicted vessel masks; export prediction labels.

## Results and Lessons

- My report recorded approximately **92% training accuracy**, which should **not** be interpreted as independent test Dice, F1 or validated clinical performance.
- Class imbalance was a significant challenge: predicting mostly background could produce misleading accuracy.
- I investigated stain normalization (including Vahadane) but **did not implement it in the final pipeline**, due to dependency and compatibility concerns for PAS-stained imagery.
- This assignment taught me how to design a reproducible image-analysis workflow, interpret failures, and evaluate preprocessing choices.

## Original Materials

- `hw1_SegmentMicrovascular.mlx` — original MATLAB Live Script (available from my coursework archive; not yet published here).
- `trainedModel2025-04-02-14-10.mat` — saved trained model (not yet published here).
- `醫學影像分析專題hw1.pdf` — original report with workflow, code commentary and prediction images (pending review and upload).

**Data and attribution:** This is a learning project, not an official Kaggle competition submission or a clinical study. Dataset files are not redistributed here. Inspired by [HuBMAP — Hacking the Human Vasculature](https://www.kaggle.com/competitions/hubmap-hacking-the-human-vasculature).

## What I'd improve now

- Split by original image/WSI before augmentation, to prevent related augmented samples from appearing in both training and validation.
- Evaluate with vessel-specific **Dice/IoU** on held-out images rather than relying on aggregate accuracy.
- Document the label-export format and verify that output matches the required specification.
- Test stain-normalization choices specifically for PAS images, rather than assuming H&E-oriented procedures generalize.

*These are retrospective improvement ideas, not experiments claimed to have been completed.*
