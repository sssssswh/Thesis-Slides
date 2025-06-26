# 🌳 YOLO Models for Instance Segmentation of Individual Tree Crowns from Aerial Imagery in Wellington

## 📋 Overview

This repository contains the PhD thesis defense slides for research on developing innovative YOLO-based models for instance segmentation and species classification of individual tree crowns from aerial imagery, with a focus on Wellington, New Zealand. 🇳🇿

**👨‍🎓 Author:** Ziyi Sun  
**👨‍🏫 Supervisors:** Bing Xue and Mengjie Zhang  
**🏛️ Institution:** School of Engineering and Computer Science, Victoria University of Wellington


## 🎯 Research Motivation

The research addresses critical environmental challenges in the Wellington region:
- **Landslide Prevention:** Supporting reforestation efforts in the Wairarapa area to prevent landslides
- **Strategic Tree Planting:** Determining optimal locations for new tree plantings
- **Species Selection:** Identifying which tree types work best for specific environmental conditions

## 🎯 Technical Approach

### Instance Segmentation Goals
The research tackles three key computer vision tasks:
1. **Classification:** Assign class labels to each tree canopy
2. **Detection:** Locate canopies using bounding boxes  
3. **Segmentation:** Provide precise canopy shapes within detected areas

### Key Challenges
- Dense forest stands with overlapping and shaded canopies
- Complex tree crown characteristics (size, color, shape, texture variations)
- Small object detection in aerial imagery
- False positive identification from background elements (shrubs, grass, weeds)
- Data labeling uncertainties

## 🎯 Major Contributions

### 1. YOLO-ITC
- **Innovation:** Dense blocks with efficient attention mechanisms
- **Focus:** Enhanced feature extraction for complex canopy environments
- **Optimization:** Reconfigured large-object detection for medium-scale canopies

### 2. YOLOv8E
- **Innovation:** Two novel candidate positive sample selection schemes
- **Focus:** Improved detection of small tree canopies
- **Efficiency:** Lightweight design with reduced computational requirements

### 3. YOLOv8-FF
- **Innovation:** Feature fusion-enhanced architecture
- **Focus:** Cross-scale and same-scale fusion techniques
- **Enhancement:** Large-kernel convolutions for better global context

## 🎯 Performance Results

| Method | Box AP | Mask AP | AP50 | AP75 | APS | APM | FLOPs | #Params |
|--------|--------|---------|------|------|-----|-----|-------|---------|
| YOLO-ITC | 36.2 | 32.0 | 60.3 | 31.7 | 30.8 | 45.3 | 141.8G | 82.2M |
| YOLOv8E-A | 36.0 | 32.1 | 60.7 | 32.2 | 30.9 | **45.4** | 106.4G | 56.9M |
| YOLOv8E-B | 36.1 | 32.2 | 60.5 | 31.9 | 31.2 | 43.7 | 106.4G | 56.9M |
| YOLOv8-FF | **37.6** | **32.9** | **61.4** | **32.8** | **31.9** | 44.6 | 196.1G | 54.4M |

## 🎯 Publications

This research has resulted in multiple peer-reviewed publications:

1. **Ziyi Sun**, Bing Xue, Mengjie Zhang, and Jan Schindler. "Feature Fusion to Improve YOLOv8 for Segmenting and Classifying Aerial Images of Tree Crowns." *IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing* (2025): 1-14.

2. **Ziyi Sun**, Bing Xue, Mengjie Zhang, and Jan Schindler. "YOLO-ITC: A New YOLO Method for Instance Segmentation of Individual Tree Crowns." *IEEE Transactions on Emerging Topics in Computational Intelligence* (2025): 1-15.

3. **Ziyi Sun**, Bing Xue, Mengjie Zhang, and Jan Schindler. "YOLOv8E: an efficient YOLOv8 method for instance segmentation of individual tree crowns in Wellington City, New Zealand." *Journal of the Royal Society of New Zealand* (2024): 1-26.

4. **Ziyi Sun**, Bing Xue, Mengjie Zhang, and Jan Schindler. "An Improved Mask R-CNN for Instance Segmentation of Tree Crowns in Aerial Imagery." *2023 38th International Conference on Image and Vision Computing New Zealand (IVCNZ)*, 2023.

## 🎯 Future Work

- Handling overlapping and ambiguously bounded tree crowns
- Improving model generalization across different regions
- Incorporating multi-sensor and multi-spectral data
- Exploring transformer-based architectures
- Implementing semi-supervised and active learning approaches
- Real-time and on-device deployment
- Neural architecture search optimization

## 🎯 Applications

This research has direct applications in:
- **Environmental Management:** Forest monitoring and conservation
- **Urban Planning:** Green infrastructure development
- **Climate Action:** Carbon sequestration assessment
- **Disaster Prevention:** Landslide risk mitigation through strategic reforestation

---

*This research contributes to the intersection of computer vision, environmental science, and sustainable development, providing tools for better forest management and environmental protection in New Zealand.*
