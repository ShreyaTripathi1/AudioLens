# AudioLens - Object Detection for the Visually Impaired
Bringing Vision to Voice


AudioLens is an assistive tool designed to help visually impaired individuals understand their surroundings through real-time object detection and audio descriptions. It identifies objects using advanced computer vision models (YOLO) and describes them aloud, providing distance and direction for better spatial awareness.

---

# Features
- 🎯 **Real-Time Object Detection** using YOLOv8x  
- 📏 **Distance Estimation** to help gauge how far objects are  
- 🔊 **Voice Descriptions** via Text-to-Speech (TTS)  
- 🧠 **Smart Summarization** with NLP for concise, natural explanations  
- 📸 **Camera Integration** for real-time analysis

- ---

### Recommended YOLO Versions for Better Accuracy:
-> YOLOv8 (Larger Models)

- yolov8s.pt (Small) – Better than yolov8n.pt but still fast.

- yolov8m.pt (Medium) – Good balance between speed and accuracy.

- yolov8l.pt (Large) – High accuracy, slower on low-end devices.

- yolov8x.pt (Extra Large) – Best accuracy, but resource-intensive.
      
      
-> YOLOv5 (Stable & Popular)

- yolov5s.pt, yolov5m.pt, yolov5l.pt, yolov5x.pt 

Lightweight and great for real-time applications.
      
      
-> YOLOv7 (High Performance for Real-Time Tasks) 

- Excellent speed-accuracy trade-off for complex tasks.

---

### Install All Dependencies:
```
pip install -r requirements.txt
```
