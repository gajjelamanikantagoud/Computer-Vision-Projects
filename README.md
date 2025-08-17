# Computer-Vision-Projects
Welcome to the Computer Vision Projects Repository, a curated collection of practical and innovative projects demonstrating various aspects of computer vision technology. This repository is ideal for learners, developers, and researchers interested in exploring how machines interpret and analyze visual data to solve real-world problems.
<!DOCTYPE html>
<html lang="en">
<body>

<h1>Project 1 - 👋 Hand Gesture Controlled Screen Brightness</h1>

<h2>📌 Project Overview</h2>
<p>This project implements a <span class="highlight">computer vision-based system</span> that dynamically controls your laptop or PC screen brightness using <span class="highlight">hand gestures</span> detected via the webcam. It leverages Google's <code>MediaPipe Hands</code> model to track finger landmarks and adjusts brightness based on the distance between the <strong>thumb</strong> and <strong>index finger</strong>.</p>

<hr/>

<h2>🧠 Problem Statement</h2>
<p>Traditional brightness adjustment requires manual input (keyboard shortcuts or system settings). This project introduces a more <em>intuitive and touch-free control mechanism</em>:</p>
<ul>
  <li>Control screen brightness by moving your thumb and index finger closer or farther apart.</li>
  <li>Enhances <strong>accessibility</strong> and <strong>user experience</strong> in various lighting environments.</li>
</ul>

<hr/>

<h2>🛠️ Technologies Used</h2>
<ul>
  <li>Python</li>
  <li>OpenCV (for video capture and image processing)</li>
  <li>MediaPipe (for hand landmark detection)</li>
  <li>NumPy (for mathematical computations)</li>
  <li>screen-brightness-control (to programmatically set screen brightness)</li>
</ul>

<hr/>

<h2>🔍 Workflow</h2>
<ol>
  <li>Capture webcam video with OpenCV.</li>
  <li>Detect hand landmarks using MediaPipe Hands.</li>
  <li>Calculate distance between thumb tip and index finger tip.</li>
  <li>Map this distance linearly to screen brightness levels (0–100%).</li>
  <li>Adjust screen brightness using <code>screen-brightness-control</code>.</li>
</ol>

<hr/>

<h2>📊 Results & Observations</h2>
<ul>
  <li>Brightness control is <strong>smooth and responsive</strong> when adjusting fingers.</li>
  <li>Finger <strong>pinch distance</strong> maps linearly from <code>30px</code> (min brightness) to <code>200px</code> (max brightness).</li>
  <li><strong>Fist gesture</strong> controls mute/unmute (threshold adjustable for partial finger folds).</li>
  <li><strong>Open palm gesture</strong> triggers app switching.</li>
  <li>Gesture detection is sensitive to lighting and camera position; user calibration recommended.</li>
  <li><strong>Press 'q' to stop detection.</li>
    <img width="809" height="633" alt="Screenshot 2025-08-17 155221" src="https://github.com/user-attachments/assets/e0048186-8199-48c8-a04a-590b8cbf9056" />

</ul>

<hr/>

<h2>▶️ How to Run (Jupyter Notebook)</h2>
<ol>
  <li>Clone the repository:<br />
    <code>git clone https://github.com/your-username/hand-gesture-brightness.git</code><br />
    <code>cd hand-gesture-brightness</code>
  </li>
  <li>Install required packages (inside the notebook or terminal):<br />
    <code>!pip install opencv-python mediapipe numpy screen-brightness-control PyQt5</code>
  </li>
  <li>Open <strong>Jupyter Notebook</strong> and create a new Python notebook.</li>
  <li>Copy the main logic (hand landmark capture, gesture detection, and control code) into the notebook cell and execute.<br />
    <em>Example first cell:</em>
    <pre><code>
import cv2
import mediapipe as mp
import numpy as np
import screen_brightness_control as sbc
# (Paste additional logic here)
    </code></pre>
  </li>
  <li>
    When you run the notebook cell, grant camera access and follow the instructions to use hand gestures for brightness and controls.
  </li>
</ol>
<p>

</p>


<h2>✅ Future Enhancements</h2>
<ul>
  <li>More complex gesture recognition for volume control and media playback.</li>
  <li>Multi-hand gesture support with independent controls.</li>
  <li>Calibration wizard to automate gestures sensitivity based on user environment.</li>
  <li>Smart home IoT integration for environmental control.</li>
</ul>

<hr/>

<h2>📂 Project Genre</h2>
<ul>
  <li>Computer Vision (CV)</li>
  <li>Human-Computer Interaction (HCI)</li>
  <li>Utilizes Deep Learning (MediaPipe pre-trained model internally)</li>
</ul>

<hr/>

</body>
</html>
