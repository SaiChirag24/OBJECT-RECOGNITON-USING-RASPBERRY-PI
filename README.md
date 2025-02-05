# OBJECT-RECOGNITON-USING-RASPBERRY-PI

This project implements a real-time object detection system using Raspberry Pi 3B+, OpenCV, and SSD MobileNet. It detects objects from a live camera feed and provides confidence-based LED feedback using Raspberry Pi's GPIO pins.


🎯 Features:

📷 Real-time object detection using OpenCV and SSD MobileNet.

🔴🟢 LED indication based on detection confidence:

Red LED (GPIO 18) blinks if confidence is below 50%.

Green LED (GPIO 23) blinks if confidence is above 50%.

🎯 Optimized for Raspberry Pi to ensure smooth performance.


🛠️ Setup and Installation:


1️⃣ Clone the Repository

    DOWNLOAD ZIP
    
2️⃣ Install Dependencies

    Ensure your Raspberry Pi has the required libraries:
    
    sudo apt update && sudo apt upgrade -y
    
    pip install opencv-python numpy RPi.GPIO
    
3️⃣ Download Model Files

    Download the SSD MobileNet v3 COCO model and place them in the model folder:
    
    ssd_mobilenet_v3_large_coco_2020_01_14.pbtxt
    
    frozen_inference_graph.pb

4️⃣ Run the Detection Script

    python object_detection.py
    
    
🖥️ How It Works

The camera captures real-time video.

Objects are detected using SSD MobileNet.

If an object's confidence score is above 50%, the green LED blinks.

If confidence is below 50%, the red LED blinks.


🛠 Hardware Requirements:

Raspberry Pi 3B+ (or later)

Raspberry Pi Camera Module

Two LEDs (Red & Green)

Resistors (330Ω)

Breadboard & Jumper Wires

📜 License
This project is open-source under the MIT License.
