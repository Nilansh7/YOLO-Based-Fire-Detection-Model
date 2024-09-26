# **YOLO-Based Fire Detection Model: Heading Towards Enhanced Safety**
🚨 Overview
This project implements a YOLO (You Only Look Once) deep learning model for fire detection, aiming to enhance safety by providing early alerts in the event of a fire. Leveraging YOLO's real-time object detection capabilities, the model identifies potential fire hazards in images or video streams, making it suitable for surveillance systems, fire safety management, and emergency response.


🔥 Features
Real-time Fire Detection: Efficient detection of fire in both images and video streams.
High Accuracy: YOLOv5 is known for its precision and ability to minimize false positives.
Lightweight Model: Can be deployed on devices with limited computational resources.
Versatile Input: Works with both static images and live video streams.
Customizable: Easily trainable on custom datasets to improve performance for specific environments.

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



IV. 🙌 Contributing
Contributions are welcome! If you'd like to improve the model or add new features, feel free to 

Fork the repository
Create a new branch (git checkout -b feature-branch)
Commit your changes (git commit -m 'Add new feature')
Push to the branch (git push origin feature-branch)
Open a pull request


V. 📄 License
This project is licensed under the MIT License. See the LICENSE file for details.

VI. 💬 Contact
For any questions or suggestions, feel free to open an issue or reach out at s.nilansh07@gmail.com.

VII. 🔗 Additional Resources:
YOLOv5 GitHub Repository
Fire Dataset for Object Detection
