+++
title = 'Wearable Risk Awareness System'
icon = "fa-solid fa-shirt"
description = "A sensor-based wearable system that helps workers recognize ergonomic risks through real-time feedback."
startDate = "2026-02-19"
endDate = "2026-04-24"
github = "https://github.com/Noisyboy-9/ergonomic_pose_detector"
+++

## Project Overview
This is an Ergonomic Risk Awareness System designed to detect whether workers are using dangerous postures during lifting. It is an edge-computing wearable device that provides real-time posture detection and delivers delayed vibration feedback, gently alerting workers to hazardous postures only when necessary, effectively preventing injuries while minimizing workflow disruption.
## The Problem & Motivation
Occupational musculoskeletal disorders (MSDs), particularly low back pain, are a major global health challenge. In the European context, work-related MSDs account for over 40% of all work-related health problems and are a primary cause of sick leave and early retirement among manual workers.  

However, current wearable devices often vibrate continuously, which can distract workers or lead them to ignore the device altogether. Therefore, our goal was to develop a system that accurately detects hazardous postures but delivers progressive alerts "only when truly necessary," aiming to improve workers' willingness to wear the device long-term.

## The Product
The wearable ergonomic risk awareness system is built around a three-layer pipeline transforming raw inertial sensor data into real-time haptic feedback. 
- **The sensing layer** consists of four MPU6050 IMU sensors at the hip, lower back (abbreviated as: LB), upper back (abbreviated as: UB), and neck. 
- **The processing layer** runs entirely on the ESP32-S3 microcontroller with no external connectivity. 
- **The feedback layer** delivers alerts through a vibration motor and LED whenever an unsafe posture is sustained for more than a configurable time threshold t<sub>1</sub>.

### The Vest
#### From Concept to Reality
Initially, we attached the IMU sensors directly to various body parts to test the measurement feasibility. However, we quickly realized this setup was highly inconvenient and impractical for daily industrial use. To solve this, we developed a custom ergonomic vest to seamlessly integrate all hardware.

<div style="display: flex; gap: 15px; align-items: stretch; justify-content: center; width: 100%; margin-top: 15px; margin-bottom: 30px;">
  
  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/RiskAwarenessWearable/vestIdea.jpg" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/RiskAwarenessWearable/vestIdea.jpg" alt="First Prototype" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer; display: block; margin: 0 auto;">
    </a>
    <div style="margin-top: 12px; margin-bottom: 0;">
      <p style="font-size: 1em; font-weight: bold; color: #333; margin: 0;">First Prototype</p>
      <p style="font-size: 0.85em; color: #666; margin: 4px 0 0 0; line-height: 1.4;">Initial setup with exposed wires.</p>
    </div>
  </div>

  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/RiskAwarenessWearable/vestBack.jpg" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/RiskAwarenessWearable/vestBack.jpg" alt="Vest Back" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer; display: block; margin: 0 auto;">
    </a>
    <div style="margin-top: 12px; margin-bottom: 0;">
      <p style="font-size: 1em; font-weight: bold; color: #333; margin: 0;">Vest Back</p>
      <p style="font-size: 0.85em; color: #666; margin: 4px 0 0 0; line-height: 1.4;">Hardware fully integrated.</p>
    </div>
  </div>

  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/RiskAwarenessWearable/vestFront.jpg" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/RiskAwarenessWearable/vestFront.jpg" alt="Vest Front" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer; display: block; margin: 0 auto;">
    </a>
    <div style="margin-top: 12px; margin-bottom: 0;">
      <p style="font-size: 1em; font-weight: bold; color: #333; margin: 0;">Vest Front</p>
      <p style="font-size: 0.85em; color: #666; margin: 4px 0 0 0; line-height: 1.4;">Adjustable and easy to wear.</p>
    </div>
  </div>

</div>

#### Final Design

<div style="display: flex; gap: 20px; align-items: stretch; justify-content: center; width: 100%;">
  
  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/RiskAwarenessWearable/vest.png" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/RiskAwarenessWearable/vest.png" alt="Vest Prototype" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer;">
    </a>
    <p style="font-size: 0.9em; color: #555; margin-top: 8px; margin-bottom: 0;">Wearable Vest</p>
  </div>

  <div style="flex: 1; display: flex; flex-direction: column; justify-content: space-between; text-align: center;">
    <a href="/image/RiskAwarenessWearable/circuit.png" target="_blank" style="text-decoration: none; border: none; box-shadow: none; outline: none; display: block;">
      <img src="/image/RiskAwarenessWearable/circuit.png" alt="Circuit schematic" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer;">
    </a>
    <p style="font-size: 0.9em; color: #555; margin-top: 8px; margin-bottom: 0;">Circuit Schematic</p>
  </div>

</div>

The final physical design prioritizes usability and measurement reliability through three key features:
* **Snug Fit for Accuracy:** The vest is designed to fit tightly against the body. This minimizes fabric movement and ensures the IMU sensors accurately capture true spinal kinematics without signal noise.
* **Adjustable Sensor Placement:** To accommodate workers of different heights and body shapes, the vest allows for flexible adjustment of the IMU positions. This ensures the sensors are always correctly aligned with the user's specific neck, back, and hip nodes.
* **Easy Donning and Doffing:** Recognizing the fast-paced nature of manual labor, the vest is designed to be as easy to put on and take off as standard workwear, adding zero hassle to the worker's daily routine.

### The System
To address the computational constraints of wearable edge devices while ensuring real-time responsiveness, our system architecture utilizes a dual-mode approach: a rule-based Finite State Machine (FSM) and a lightweight Machine Learning (ML) classifier.

#### Finite State Machine (FSM)
To ensure the system operates reliably and in real-time on the edge, we designed an FSM to classify various working postures. Compared to resource-heavy algorithms, the FSM delivers accurate classifications with minimal latency.

![FSM State Transition Diagram](/image/RiskAwarenessWearable/FSM_Diagram.png)
By calculating the "trunk flexion" and "relative angle differences" from the multi-node sensors, the system instantly categorizes the user's movement into the following states:
- Standing: The baseline state of the system where all sensors are near zero, triggering no alerts.
- Bending: Detects normal trunk flexion. It is considered a safe short-term posture and triggers no feedback.
- Slouching: Detects abnormal rounding of the upper back while the hip stays upright. If sustained beyond the time threshold (t<sub>1</sub>= 5s), it triggers a **short vibration pulse (300ms)** as a gentle reminder.
- Deep Bend: Detects a dangerous angle that places heavy compressive load on the spine. If prolonged, it triggers a **long vibration pulse (800ms)** as a strong warning.  

#### Machine Learning Classifier

To complement the rule-based FSM, we implemented a lightweight machine learning (ML) classifier to process the IMU data and classify three primary states: standing, bending, and slouching. 

* **Feature Engineering (FFT):** Raw IMU signals were pre-processed using a 32-point Fast Fourier Transform (FFT) to convert time-domain signals into the frequency domain. This generated an input layer of 504 spectral features, which reduced noise sensitivity and improved class separability.
* **Model Selection (FNN):** A Feedforward Neural Network (FNN) with four fully connected hidden layers was trained for 60 epochs. An FNN was deliberately selected over heavier CNNs or RNNs to balance classification capability with the computational efficiency required for the ESP32.
* **Edge Optimization (INT8 Quantization):** To meet hardware memory constraints, the model was quantized to INT8 precision before deployment. This optimization significantly reduced the model footprint, enabling real-time inference within milliseconds directly on the edge microcontroller.

## Results
The system's performance was evaluated based on both the real-time reliability of the FSM and the classification accuracy of the ML model running on the ESP32-S3 edge device.

### FSM Performance
* **Reliable Real-Time Tracking:** Across all testing sessions, the FSM transitions correctly matched the expected posture conditions without any misclassifications in the observed scenarios.
* **Controlled Latency:** The system maintained a short response delay of 200-500 ms. This intentional delay, caused by a low-pass filter and stabilization period, successfully eliminated hardware spikes and rapid oscillations at the cost of a slight, acceptable lag.

### Machine Learning Performance
* **Accuracy & Metrics:** The final INT8 quantized model achieved a validation accuracy of 74.2%, with a weighted average F1-score, precision, and recall all at 0.74. 
* **Inference Speed:** The model successfully performed inference within milliseconds directly on the ESP32, confirming its suitability for near real-time feedback.
* **Class Separability:** The model showed strong performance in distinguishing standing from dynamic postures. The primary confusion occurred between bending and slouching, as both involve similar forward trunk inclinations and overlapping spectral features.

<div style="display: flex; gap: 20px; align-items: stretch; justify-content: center; width: 100%; margin-top: 20px; margin-bottom: 30px;">
  
  <div style="flex: 1; display: flex; flex-direction: column; text-align: center;">
    <a href="/image/RiskAwarenessWearable/confusionMatrix.png" target="_blank" style="text-decoration: none; border: none;">
      <img src="/image/RiskAwarenessWearable/confusionMatrix.png" alt="Confusion Matrix" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer;">
    </a>
    <p style="font-size: 0.9em; color: #555; margin-top: 8px;">Confusion Matrix (Validation Set)</p>
  </div>

  <div style="flex: 1; display: flex; flex-direction: column; text-align: center;">
    <a href="/image/RiskAwarenessWearable/matrix.png" target="_blank" style="text-decoration: none; border: none;">
      <img src="/image/RiskAwarenessWearable/matrix.png" alt="Metrics Table" style="width: 100%; height: auto; border-radius: 8px; cursor: pointer;">
    </a>
    <p style="font-size: 0.9em; color: #555; margin-top: 8px;">Model Performance Metrics</p>
  </div>

</div>



---

## Tech Stack

### **Hardware / Firmware**
* **Controller**: ESP32-S3 (XIAO ESP32-S3).
* **Sensor**: 4x MPU6050 6-axis IMUs.
* **Component**: TCA9548A I2C Multiplexer, Vibration Motor, LED.
* **Protocol**: I2C (40 kHz).

### **Software / Edge AI**
* **Architecture**: Finite State Machine (FSM), Feedforward Neural Network (FNN).
* **Data Processing**: 32-point FFT, Low-pass filter.
* **Optimization**: INT8 Quantization.

---

## Contributions
* **Preliminary Research (Collaborative):** Reviewed biomechanical fatigue models to identify key ergonomic issues.
* **Concept Development (Collaborative):** Translated academic research into proactive posture intervention strategies.
* **Product Design:** Designed an adjustable vest for diverse body types, ensuring accurate sensor placement and discreet haptic feedback.
* **Data collection (Collaborative):** Performed structured movements while wearing the vest to collect motion data from the system.
* **Product Testing (Collaborative):** Tested system latency, accuracy, usability, and wearability.
---

## Team & Acknowledgments
This project received the **Best Pervasive System** of the Pervasive Computing course.

* **Team Members**: **Ming-Hua Hsieh**, Mansi Bhardwaj, Afeef Ahmed Mohamed Abdulla, Sina Shariati, Hari Sahar Ravi Kumar, and Andrea Battarelli Martini.
* **Supervisor**: Özlem Durmaz Incel
* **Institution**: University of Twente (UT), Enschede, the Netherlands

![Certificate](/image/RiskAwarenessWearable/Certificate.jpg)

[Explore the Code on GitHub](https://github.com/Noisyboy-9/ergonomic_pose_detector)