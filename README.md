# TinyML-Based-Gunshot-and-Emergency-Sound-Detection-on-Edge-Devices

This project explores how TinyML can be used to detect gunshots and emergency sirens in real time using edge devices such as the Arduino Nano 33 BLE Sense. The system processes audio locally and classifies sounds using a lightweight machine learning model built on Edge Impulse, enabling privacy-preserving and fast emergency detection in sensitive environments.

**Problem Addressed:**
Traditional emergency sound detection systems require internet connectivity and cloud processing, introducing latency and privacy risks. This project solves that by bringing intelligent audio classification directly to low-power microcontrollers.

**Tools and Technologies:**

* Edge Impulse (model training and deployment)
* TensorFlow Lite for Microcontrollers
* Arduino Nano 33 BLE Sense
* ESC-50 and UrbanSound8K datasets
* MFCC (Mel-Frequency Cepstral Coefficients)
* Python (for data preparation)

**System Architecture:**

* Input: 1-second audio clips (16kHz)
* Feature Extraction: MFCCs
* Model: Lightweight CNN or dense neural network
* Output: Predicted label – gunshot, siren, or background noise
* Deployment: Compiled with TensorFlow Lite and uploaded to a microcontroller

**Model Training and Evaluation:**

* Dataset split 80/20 for training/testing
* Data augmented with noise, pitch shift, and time stretch
* Model optimized for edge constraints such as size and latency
* Evaluation metrics included precision, recall, F1-score, and confusion matrix
* Edge Impulse tools used for deployment tuning

**Results:**

* Low-latency detection on edge device
* Accurate classification across real-world sound samples
* Works fully offline, suitable for schools, transport hubs, and public areas
* Compliant with Responsible AI licensing, with no data storage or surveillance

**Future Improvements:**

* Enhance detection with more diverse real-world data
* Add real-time alert notifications using LEDs or wireless communication
* Test across varied environments for robustness
* Explore deployment on other microcontrollers or mobile platforms
