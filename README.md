
<img width="408" height="221" alt="image" src="https://github.com/user-attachments/assets/5b633193-39a8-4b65-a7bc-8fd9879ccbd9" />



Drishti AI Smart Glass 👓

Vision for the Visually Impaired

Drishti AI Smart Glass is an affordable AI-powered wearable system designed to help blind and visually impaired people understand and navigate their surroundings using real-time image recognition and voice feedback.

The system uses an ESP32-CAM to capture images and Google Gemini AI to analyze the scene and respond with short voice guidance for the user.

🌍 Problem Statement

Millions of visually impaired people face daily challenges such as:

Identifying objects in front of them
Reading text and signboards
Understanding surroundings independently
Navigating safely in unknown environments

Existing assistive solutions are expensive and not easily accessible.
Drishti AI Smart Glass aims to provide a low-cost and smart wearable alternative.

💡 Solution Overview

Drishti AI Smart Glass is a real-time vision assistant that:

Captures the environment using a tiny camera mounted on glasses
Sends the image to a server via Wi-Fi
Uses Google Gemini Vision AI to understand the scene
Converts the response into voice guidance
Speaks the answer to the user through earphones

This allows blind users to simply ask:

“What is in front of me?”

…and hear a short, accurate response instantly.

🧠 Technologies Used
Hardware
ESP32-CAM (Camera + Wi-Fi module)
Smart Glass Frame
Earphones / Speaker
Software & AI
Python (Flask Server)
OpenCV (Image capture & streaming)
Speech Recognition (Voice input)
Text-to-Speech (Voice output)
Google Gemini Vision API (Scene understanding)
⚙️ System Architecture
Step-by-Step Working

1️⃣ Voice Trigger

User asks a question using a wake word
Example: “Hey Drishti, what’s in front of me?”

2️⃣ Image Capture

ESP32-CAM captures a real-time image.

3️⃣ Image Transmission

Image is sent via Wi-Fi to the Python server.

4️⃣ AI Processing

Server sends image + user question to Google Gemini Vision.

5️⃣ Smart Response

Gemini analyzes the scene and generates a short answer.

6️⃣ Voice Feedback

The response is converted to speech and played to the user.
✨ Key Features
🟢 Real-Time Object Detection

Identifies everyday objects such as:

People
Vehicles
Doors
Chairs
Stairs
🎨 Color Identification

Example:

“The shirt is red.”
🔤 Text Recognition (OCR)

Reads:

Signboards
Labels
Product names
🎤 Voice-Based Interaction

Hands-free operation using speech input and output.

💰 Low-Cost Wearable

Uses affordable and easily available components.

🖥️ Project Structure
Drishti-AI-Smart-Glass/
│
├── app.py                # Main Flask server
├── esp32_cam_code/      # ESP32 camera streaming code
├── templates/           # Web interface (optional)
├── static/              # Images & assets
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
