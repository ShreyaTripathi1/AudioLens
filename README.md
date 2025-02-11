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

---

## *Technologies Used*  

1. **Image Capturing:**  
   - **Used:** JavaScript (`navigator.mediaDevices.getUserMedia`) with Python (`eval_js`) in Colab.  
   - **Explanation:** Since Colab runs in a browser, we can’t access the webcam directly with Python. Instead, we use JavaScript to activate the webcam and capture images, which are then processed by Python for object detection.  

2. **Object Detection:**  
   - **Used:** YOLO (You Only Look Once) Model from the `ultralytics` library.  
   - **Explanation:** YOLO processes the captured images to detect objects in real time, identifying their class, position, and bounding boxes.  

3. **Text-to-Speech (TTS):**  
   - **Used:** `gTTS` (Google Text-to-Speech).  
   - **Explanation:** Converts the detected object descriptions into spoken words, providing audio feedback for visually impaired users. It’s preferred for its natural-sounding voice.  

4. **Text Generation:**  
   - **Used:** `transformers` library with `facebook/bart-large-cnn` model.  
   - **Explanation:** Summarizes the detected objects into coherent sentences before converting them to speech, making the descriptions more natural and easy to understand.
