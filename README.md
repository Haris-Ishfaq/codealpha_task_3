# Real-Time Object Detection and Tracking with YOLOv8 and DeepSORT

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1z_3JWafZv-dwCHps2NYa0fGaGMcI-yjk)

## Overview

This Colab notebook provides a complete implementation for real-time object detection and tracking using:
- **YOLOv8** for state-of-the-art object detection
- **DeepSORT** for robust object tracking
- **OpenCV** for video processing

The solution works with:
- Live webcam feeds
- Uploaded video files
- Static images

## Features

- 🚀 Real-time performance (adjustable based on model size)
- 🔍 Multiple input source support
- 🆔 Persistent object tracking with IDs
- 📊 Customizable detection parameters
- 💾 Results saving capability

## Quick Start

1. Click the "Open in Colab" button above
2. Run all cells sequentially
3. Choose your input source:
   - Webcam (default)
   - Upload a video file (if webcam unavailable)
   - Test with sample image

## Notebook Structure

1. **Environment Setup**
   - Install required packages
   - Import dependencies

2. **Model Initialization**
   - Load YOLOv8 model (default: yolov8n.pt)
   - Configure DeepSORT tracker

3. **Processing Pipeline**
   - Webcam/video capture setup
   - Frame-by-frame processing
   - Visualization of results

4. **Utilities**
   - Image detection example
   - Performance metrics

## Configuration Options

| Parameter | Description | Default Value |
|-----------|-------------|---------------|
| `model_size` | YOLOv8 model variant (n/s/m/l/x) | `n` |
| `max_age` | DeepSORT track duration without detection | `30` |
| `conf_threshold` | Minimum detection confidence | `0.5` |

## Troubleshooting

### Webcam Not Working?
1. Check Colab's camera permissions
2. Try refreshing the runtime
3. Use the fallback video upload option

### Performance Issues?
1. Switch to smaller YOLO model (yolov8n)
2. Reduce frame resolution
3. Disable unnecessary visualizations

## Examples

**Webcam Tracking**  
![Webcam Demo](https://via.placeholder.com/600x400/000000/FFFFFF?text=Webcam+Tracking+Demo)

**Video File Processing**  
![Video Demo](https://via.placeholder.com/600x400/000000/FFFFFF?text=Video+Processing+Demo)
