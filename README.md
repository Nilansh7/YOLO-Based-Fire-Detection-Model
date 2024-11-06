# **YOLO-Based Fire Detection Model: Heading Towards Enhanced Safety**
🚨 Overview
This project implements a YOLO (You Only Look Once) deep learning model for fire detection, aiming to enhance safety by providing early alerts in the event of a fire. Leveraging YOLO's real-time object detection capabilities, the model identifies potential fire hazards in images or video streams, making it suitable for surveillance systems, fire safety management, and emergency response.

🚀 Getting Started

1. Clone the Repository:
git clone [https://github.com/your-username/fire-detection-yolo.git](https://github.com/Nilansh7/YOLO-Based-Fire-Detection-Model)
cd fire-detection-yolo

3. Install Dependencies:
Ensure you have Python 3.7+ and pip installed. Then, install the required libraries:
pip install -r requirements.txt

3. Download Pre-trained Weights:
Download the pre-trained YOLOv5 weights from the official repository or use your own.

4. Run Fire Detection on an Image:
python detect.py --source data/images/fire_test.jpg --weights yolov5s.pt --conf 0.4

6. Run Fire Detection on a Video Stream:
python detect.py --source data/videos/fire_test.mp4 --weights yolov5s.pt --conf 0.4


I. 🔧 Training the Model on Custom Data
Prepare Dataset: Collect fire and non-fire images, annotate them in YOLO format, and split them into training and validation sets.
Modify Configs: Update data.yaml with the path to your custom dataset.


II. **Train the Model:**
python train.py --img 640 --batch 16 --epochs 50 --data ./data.yaml --weights yolov5s.pt


III. **📊 Results & Performance**
Model Accuracy: Achieved on the test dataset.
Speed: Detects fire in real-time on images and videos at high resolution.
Include some demo screenshots or video gifs.


# MAIN:- 

1. Project Overview

    Developed a real-time fire and smoke detection system using YOLOv8 to identify fire and smoke in video frames.
    Purpose: Created to improve safety monitoring by detecting fire or smoke quickly in various environments.

Potential Question: Why did you choose YOLOv8 for this project?
Answer: YOLOv8 offers state-of-the-art accuracy and speed, essential for real-time detection tasks.
2. Dataset Preparation

    Used Roboflow to collect and annotate a custom dataset with fire and smoke images.
    Integrated Roboflow API to automate data download and management, improving efficiency.

Potential Question: How did you handle data annotation?
Answer: Roboflow’s annotation tools allowed for quick and consistent labeling, which was crucial for training a reliable model.
3. Model Training and Optimization

    Fine-tuned a pre-trained YOLOv8 model with the custom dataset, achieving high mean Average Precision (mAP) scores and low loss.
    Applied various techniques to improve model performance, including adjusting hyperparameters and validating with a train-test-validation split.

Potential Question: How did you measure model accuracy?
Answer: We measured performance using mAP, which reflects the precision and recall balance, and ensured low loss across datasets.
4. Inference and Real-Time Implementation

    Deployed the model for inference with GPU acceleration using CUDA, enabling it to process video frames in real time.
    Used CLI commands to execute predictions and save annotated frames, providing visual verification of detections.

Potential Question: What challenges did you face in real-time deployment?
Answer: Optimizing inference speed was challenging, but leveraging CUDA for GPU acceleration made real-time detection feasible.
5. Results and Potential Applications

    The model achieved accurate detection and tracking of fire and smoke, suitable for integration into larger safety monitoring systems.
    Applications include industrial safety, forest fire monitoring, and building security.

Potential Question: How would you further improve this project?
Answer: Additional improvements could include training on diverse environmental conditions and implementing further optimizations for mobile or edge devices.
