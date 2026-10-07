---
layout: kc-page
title: "Projects"
permalink: /projects/
description: "Projects by Kimaya Chavan across computer vision, robotics, embedded systems and IoT."
redirect_from:
  - /portfolio/
---

<div class="kc-page">
<div class="kc-container">

<header class="kc-page__header">
<p class="kc-page__eyebrow">Things I’ve built</p>
<h1 class="kc-page__title">Projects</h1>
<p class="kc-page__intro">Industrial, academic and personal engineering work across computer vision, robotics, embedded systems and IoT.</p>
</header>

<section class="kc-section">
<h2>Industrial</h2>
<div class="kc-list">
<article class="kc-item">
<h3>Defense X-Ray Shell Detection &amp; Segmentation</h3>
<p>A computer vision system for detecting, counting and segmenting shells in X-ray tray imagery for automated inspection.</p>
<p class="kc-item__stack">Python · OpenCV · CVAT · YOLO</p>
<p class="kc-item__stack">Computer Vision · Perception · Physical AI — code is confidential</p>
</article>
<article class="kc-item">
<h3>IoT-Aided Smart Service Vehicle</h3>
<p>An IoT-enabled autonomous service vehicle developed for Salesforce and demonstrated across Salesforce sites in the UK and US. Designed to navigate a LEGO City environment, the vehicle combines physical sensing, ESP32/Raspberry Pi control and cloud connectivity, with Salesforce Platform Events and MQTT explored for vehicle-to-cloud communication.</p>
<p class="kc-item__stack">ESP32 · Raspberry Pi · MQTT · Salesforce Platform Events</p>
<p class="kc-item__stack">Autonomous Robotics · Industrial IoT · Embedded Systems · Cloud Integration</p>
</article>
<article class="kc-item">
<h3>CDET Automated Shell Counting System</h3>
<p>A computer-vision system developed for CDET Explosive Industries to automate the counting of blasting shells in industrial trays. The system uses dynamic tray localisation, circular-object detection, geometric filtering and multi-frame validation to produce reliable shell counts under real camera variation.</p>
<p class="kc-item__stack">Python · OpenCV · NumPy · USB Camera · JSON Configuration</p>
<p class="kc-item__stack">Computer Vision · Industrial Automation · Automated Counting · Perception</p>
</article>
</div>
</section>

<section class="kc-section">
<h2>Computer Vision &amp; AI</h2>
<div class="kc-list">
<article class="kc-item">
        <h3>
        <a href="https://github.com/kimiko-11/real-time-object-detection-tracking"
           target="_blank"
           rel="noopener noreferrer">
          Real-Time Object Detection & Tracking
        </a>
      </h3>
      <p>A real-time perception pipeline that detects and tracks multiple objects across video frames, maintaining persistent identities while visualizing trajectories and estimating short-term motion from observed velocity.</p>
      <p class="kc-item__stack">Python · YOLOv8 · OpenCV · NumPy</p>
      <p class="kc-item__stack">Object Detection · Multi-Object Tracking · Motion Analysis · Robotics Perception</p>
</article>
<article class="kc-item">
      <h3>
        <a href="https://github.com/kimiko-11/OCR-Based-Document-Understanding-System"
           target="_blank"
           rel="noopener noreferrer">
          OCR-Based Document Understanding
        </a>
      </h3>
      <p>An end-to-end document vision pipeline that converts receipt images into structured information through image preprocessing, Tesseract OCR, word-level localization and key-field extraction for company names, dates and totals.</p>
      <p class="kc-item__stack">Python · OpenCV · Tesseract OCR · NumPy · Matplotlib</p>
      <p class="kc-item__stack">Document AI · OCR · Computer Vision · Information Extraction</p>
</article>
<article class="kc-item">
        <h3>
        <a href="https://github.com/kimiko-11/Monocular-depth-object-perception"
           target="_blank"
           rel="noopener noreferrer">
          Depth-Aware Object Perception
        </a>
      </h3>
      <p>A real-time robotics perception pipeline combining YOLOv8 object detection with MiDaS monocular depth estimation to infer the relative distance of detected objects from a single RGB camera. The system generates depth visualizations and a bird's-eye obstacle map for spatial awareness.</p>
      <p class="kc-item__stack">Python · YOLOv8 · MiDaS · OpenCV</p>
      <p class="kc-item__stack">3D Perception · Object Detection · Depth Estimation · Robotics</p>
</article>
<article class="kc-item">
      <h3>
        <a href="https://github.com/kimiko-11/R-CNN-Aircraft-Detection-Selective-Search-VGG16"
           target="_blank"
           rel="noopener noreferrer">
          R-CNN Aircraft Detection
        </a>
      </h3>
      <p>An implementation of the original region-based object detection approach using Selective Search for region proposals and pretrained VGG16 features for aircraft classification. The project explores the foundations of two-stage object detection before modern end-to-end detectors.</p>
      <p class="kc-item__stack">Python · VGG16 · Selective Search · OpenCV</p>
      <p class="kc-item__stack">Object Detection · CNNs · Region Proposals · Deep Learning</p>
  </article>
  <article class="kc-item">
      <h3>
        <a href="https://github.com/kimiko-11/HCI_Dino_game"
           target="_blank"
           rel="noopener noreferrer">
          Vision-Controlled Dino Game
        </a>
      </h3>
      <p>A real-time human-computer interaction system that uses webcam-based hand tracking to control the Chrome Dino game without a keyboard. Hand landmarks are interpreted to distinguish an open hand from a closed fist and trigger the corresponding game action.</p>
      <p class="kc-item__stack">Python · OpenCV · MediaPipe · PyAutoGUI</p>
      <p class="kc-item__stack">Hand Tracking · HCI · Gesture Recognition · Real-Time Vision</p>
    </article>

</div>
</section>

<section class="kc-section">
<h2>Robotics &amp; Physical AI</h2>
<div class="kc-list">
<article class="kc-item">
<h3>ROS2 Robotics</h3>
<p>Hands-on work with ROS2 communication, publishers, subscribers, nodes and robotic system architecture.</p>
<p class="kc-item__stack">ROS2 Humble · Python · Linux</p>
</article>
</div>
</section>

<section class="kc-section">
<h2>Embedded &amp; Electronics</h2>
<div class="kc-list">
<article class="kc-item">
<h3>Interactive Floor Piano</h3>
<p>An interactive technical installation developed for a 24-hour national-level hackathon with 200+ participating teams and a ₹3 lakh+ prize pool. Built as part of the event experience, the installation used six piezoelectric floor sensors to detect footsteps and trigger musical notes in real time, creating a large-scale playable interface for attendees.</p>
<p class="kc-item__stack">Arduino Uno · Piezoelectric Sensors · Speaker · Embedded C/C++</p>
<p class="kc-item__stack">Physical Computing · Interactive Systems · Embedded Systems · Sensor Interfacing</p>
</article>
<article class="kc-item">
<h3>Interactive Target Shooter</h3>
<p>A real-time target-shooting game developed for a national-level 24-hour hackathon organised by DJS-ACM, combining IR/laser-based hit detection, target sensing, a live hit counter and countdown timer. As Head of the Technical Committee, I led the technical development and hardware integration with the team.</p>
<p class="kc-item__stack">Arduino · IR Sensors · Laser Emitter · Embedded C/C++ · Hardware Integration</p>
<p class="kc-item__stack">Embedded Systems · Interactive Hardware · Real-Time Systems · Technical Leadership</p>
</article>
</div>
</section>

<section class="kc-section">
<h2>IoT &amp; Connected Systems</h2>
<div class="kc-list">
<article class="kc-item">
<article class="kc-item">
<h3>Digital Weighing Scale</h3>
<p>A compact digital weighing system built using an Arduino Uno, load cell and HX711 amplifier, with real-time weight measurement displayed on an LCD. The system involved sensor interfacing, signal amplification, calibration against a known reference weight and embedded measurement processing.</p>
<p class="kc-item__stack">Arduino Uno · Load Cell · HX711 · LCD · Embedded C/C++</p>
<p class="kc-item__stack">Embedded Systems · Sensor Interfacing · Instrumentation · Hardware</p>
</article>
<article class="kc-item">
<h3><a href="https://github.com/kimiko-11/AeroSense" target="_blank">AeroSense</a></h3>
<p>Autonomous Obstacle-Avoiding Robot with Environmental Monitoring</p>
</article>
</div>
</section>

</div>
</div>
