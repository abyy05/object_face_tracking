#  Drone Surveillance Software

Welcome to **Drone Surveillance Software*, a Python-based real-time vision assistant that uses **OpenCV**, **speech recognition**, and **deep learning** to track **faces** and **objects** through live camera feeds — all **controlled by your voice**.

![Vision AI Banner](https://user-images.githubusercontent.com/placeholder/banner.png)

---

## 🔍 Features

- 🎤 **Voice-Controlled Interface** using Google Speech Recognition & pyttsx3  
- 🧑‍🦰 **Face Tracking** with Haar Cascade  
- 📦 **Object Detection** using SSD MobileNet (COCO model)  
- 📸 **Live Camera Streaming**  
- 🛑 **Real-time stopping & switching** between modules  
- 🧠 **Threaded execution** to keep UI responsive  

---

## 🧰 Tech Stack

- Python 3.x  
- OpenCV (cv2)  
- pyttsx3 (Text-to-Speech)  
- SpeechRecognition + Microphone  
- Pre-trained MobileNet SSD (COCO model)  
- Haarcascade Classifier  

---

## 🚀 How to Run

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/smart-vision-ai.git
cd smart-vision-ai
```

### 2. Install dependencies

```bash
pip install opencv-python numpy pyttsx3 SpeechRecognition
```

### 3. Download Model Files

- [`ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt`](https://github.com/opencv/opencv/blob/master/samples/dnn/face_detector/deploy.prototxt)
- [`frozen_inference_graph.pb`](http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v3_large_coco_2020_01_14.tar.gz)
- [`coco.names`](https://github.com/pjreddie/darknet/blob/master/data/coco.names)

Place these files in the project directory.

### 4. Add your camera URL

Edit this line in the script:

```python
camera_url = 'your camera url'  # e.g., 0 for webcam
```

### 5. Run the application

```bash
python your_script_name.py
```

---

## 🗣 Voice Commands Supported

- `"face tracking"` — Start face tracking  
- `"object tracking"` — Start object detection  
- `"stop"` — Stop the current module  
- `"exit"` — Exit the program  

---

## 💡 Lessons Learned

- Multithreading in Python for responsive interaction  
- Real-time video feed handling  
- Using pre-trained models in OpenCV DNN module  
- Integrating voice input/output with AI systems  
- Clean module switching with global state  

---

## 🎯 Example Use Case

```
Voice: "Object tracking"
>> Live camera opens with bounding boxes and labels for detected objects.

Voice: "Stop"
>> Tracking stops gracefully.

Voice: "Face tracking"
>> Camera starts detecting and highlighting faces.
```

---

## 📁 File Structure

```
📦 smart-vision-ai/
 ┣ 📄 smart_vision.py
 ┣ 📄 ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt
 ┣ 📄 frozen_inference_graph.pb
 ┣ 📄 coco.names
```

---

## 📌 Author

- **Your Name** – [GitHub Profile](https://github.com/yourusername)

---

## 📜 License

This project is licensed under the MIT License.

---


