# SafeVision — PPE Detection System

Real-time Personal Protective Equipment (PPE) detection system deployed at GICA cement factory (Meftah, Algeria). Built as a final-year engineering project at Université Blaise Pascal Blida 1.

## Results
- **84.4% mAP@0.5** on general PPE dataset
- **97.3% mAP@0.5** after fine-tuning on 1,438 factory-specific images
- Live deployment on factory floor via RTSP camera streams

## What it does
- Detects helmets, vests, gloves, and masks in real-time video streams
- Streams results to a live web dashboard via WebSocket
- Logs all detections and violations to PostgreSQL database
- Sends alerts when workers are detected without required PPE

## Tech Stack
- **Model:** YOLOv8s (Ultralytics)
- **Backend:** FastAPI + WebSocket
- **Database:** PostgreSQL
- **Streams:** RTSP camera integration
- **Training:** Custom dataset merge via Roboflow + factory fine-tuning

## Deployment
Deployed on-site at GICA industrial cement factory, Meftah, Algeria. Runs inference on live RTSP feeds from factory floor cameras.

## Team
Built by a team of 3 — Saiko, Raouf, Hocine  
