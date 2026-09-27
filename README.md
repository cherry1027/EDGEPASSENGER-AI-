# EdgePassenger AI — Edge Passenger Monitoring Lab

A lightweight two-page React research prototype demonstrating how computer-vision passenger monitoring could be optimized for resource-constrained edge hardware such as NVIDIA Jetson Nano.

> **All benchmark values are synthetic and illustrative. They were not measured on real Jetson hardware.**

## Live Demo

https://edgepassenger-ai-lab.charanvaranasi44.workers.dev/

## Features

### Passenger Monitoring

- Synthetic bus-interior camera feed
- Passenger detection bounding boxes
- Passenger count and occupancy percentage
- FPS and inference latency
- Camera selector
- Edge processing pipeline:

  `Bus Camera → OpenCV → Detection Model → TensorRT → Jetson Nano → Passenger Analytics`

### Edge Optimization Lab

Interactive configuration options:

- Models: YOLO-style Nano, MobileNet SSD, EfficientDet Lite
- Precision: FP32, FP16, INT8
- Resolution: 640×640, 416×416, 320×320
- Camera streams: 1, 2, or 4

Dynamically displays synthetic:

- Detection accuracy
- FPS
- Inference latency
- Memory usage
- GPU utilization
- Estimated power consumption
- Precision comparison chart
- Camera scalability analysis
- Recommended accuracy/latency configuration

## Technology

- React
- TypeScript
- Vinext / Vite
- Tailwind CSS
- Recharts
- Lucide icons
- Cloudflare Workers
- Wrangler
