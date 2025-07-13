Suspicious Activity Detection from Video (Action Recognition)
A deep learning model to classify videos as suspicious or normal activity based on motion and behavior patterns using CNN + LSTM.

- Project Overview
Goal: Detect and classify suspicious human activities (e.g. running, fighting, weapon-carrying) from surveillance videos.
Input: Short video clips.
Output: Suspicious / Normal label.

- Model Architecture
Frame Feature Extraction: CNN (e.g. MobileNetV2 or ResNet50 via TimeDistributed)
Temporal Modeling: LSTM layers to learn motion patterns over time
Final Output: Binary classifier (Suspicious / Normal)

- Dataset
Videos split into 2 categories:
Normal: Walking, standing, etc.
Suspicious: Running, fighting, weapon-like movements
Each video processed to extract fixed number of frames
Split: Train / Validation / Test sets

Confusion matrix and classification report available

- Files in this Repo
suspicious_activity_model.ipynb: Training and testing notebook
suspicious_activity_model.keras: Saved model
presentation.ppt: Project summary slides

- Use Cases
CCTV surveillance systems
Smart city safety
Public security automation

🛠️ Technologies Used
Python, TensorFlow / Keras
OpenCV
NumPy, Matplotlib
