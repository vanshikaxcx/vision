# SceneSpot

SceneSpot is a collection of computer vision and vision-language experiments focused on localizing and segmenting objects in images and videos using prompt-based and model-driven strategies. The repository demonstrates practical approaches to scene understanding by combining detection, segmentation, and multimodal reasoning.

---

## Project Overview

This repository contains two independent but related segmentation pipelines:

1. Prompt-guided image segmentation using vision-language cues and segmentation refinement  
2. Video-based object segmentation across frames using temporal consistency  

Both projects explore different strategies for grounding visual content and refining object boundaries in real-world scenes.

---

## Prompt-Guided Image Segmentation

This notebook focuses on segmenting objects in static images using natural language prompts.

Given an input image and a text prompt such as *"a person in white"*, the pipeline first produces an initial object localization using a vision-language model. This coarse prediction is then refined using a segmentation model to generate tighter and more accurate object boundaries.

This approach demonstrates how semantic understanding from text can be combined with pixel-level segmentation to improve localization quality. It is particularly useful in scenarios where object categories are not predefined and must be queried dynamically using language.

**Key aspects:**
- Text-driven object grounding  
- Bounding box prediction from semantic prompts  
- Segmentation refinement for accurate object masks  
- Comparison between initial and refined predictions  

---

## Video Object Segmentation

This notebook focuses on object segmentation in video sequences.

The goal is to identify and segment target objects consistently across multiple frames. The pipeline processes video data frame by frame while maintaining spatial consistency, enabling objects to be segmented over time despite motion and viewpoint changes.

This work highlights challenges such as temporal variation, movement, and partial occlusion in video understanding, and explores practical strategies for maintaining stable segmentation results.

**Key aspects:**
- Frame-wise video processing  
- Object segmentation in dynamic scenes  
- Handling motion and temporal variation  
- Foundations for video analytics and tracking systems  

---

## Extension

- Extending prompt-guided segmentation to video  
- Improving temporal consistency using tracking or memory-based approaches  
- Integrating multimodal inputs such as audio or text queries for richer scene understanding  

---

## Notes

The notebooks in this repository are experimental and research-oriented. They are intended to demonstrate problem-solving approaches and system design rather than production-ready implementations.
