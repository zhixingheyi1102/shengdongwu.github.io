---
title: "An Integrated Acquisition and Stimulation System for Closed-Loop Neuromodulation"
excerpt: "An Integrated Acquisition and Stimulation System for Closed-Loop Neuromodulation"
type: undergraduate
image: 0-cover.png
collection: projects
tags:
  - FPGA
  - STM32
  - Labview
  - Invasive BCI
priority: 1
---

This study designed and implemented an integrated acquisition and stimulation system for closed-loop brain state modulation. The system is designed to acquire microvolt-level neurophysiological signals, analyze and process them, and deliver real-time microcurrent stimulation based on the results.

The system is primarily composed of three layers: The peripheral layer utilizes the Intan RHS2116 chip, featuring 16 channels capable of simultaneous neural signal acquisition (±5mV range, 2.4 µVrms baseline noise) and microcurrent stimulation (10 nA - 2.55 mA, 8-bit DAC control). The core processing layer employs the NI myRIO platform, where its FPGA is responsible for SPI communication with the RHS2116 (50 µs command cycle), and a dual-core ARM Cortex-A9 processor handles data processing and control logic. The PC-based host software, developed using LabVIEW, is used for parameter configuration, data display, and storage.

<div class="image-row">
  <div class="image-column">
    <img src="/images/projects/undergraduate/device.png" alt="图片1描述">
  </div>
  <div class="image-column">
    <img src="/images/projects/undergraduate/stimulus.png" alt="图片2描述">
  </div>
</div>

<style>
.image-row {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin: 20px 0;
}

.image-column {
  flex: 1;
  max-width: 48%;
}

.image-column img {
  width: 100%;
  height: auto;
  border-radius: 4px;
}

/* 响应式设计：在小屏幕上切换为垂直排列 */
@media screen and (max-width: 767px) {
  .image-row {
    flex-direction: column;
  }
  
  .image-column {
    max-width: 100%;
    margin-bottom: 15px;
  }
}
</style>

In-vivo experiments were conducted in mice for system validation. Targeting the barrel cortex of CD1 mice, the system successfully acquired 4-channel LFP signals (0.1-100 Hz) at a 1000 Hz sampling rate and 16-bit resolution. It clearly recorded significant LFP changes (with main energy concentrated in the 0-20 Hz band) induced by whisker deflection at 20s and 40s, which returned to a stable state after 5s. Concurrently, the system successfully applied 10 nA microcurrent stimulation to the mice for 1s, and a pronounced LFP response was also observed. 

<div class="image-row">
  <div class="image-column">
    <img src="/images/projects/undergraduate/mouse.png" alt="图片1描述">
  </div>
  <div class="image-column">
    <img src="/images/projects/undergraduate/re.png" alt="图片2描述">
  </div>
</div>

<style>
.image-row {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin: 20px 0;
}

.image-column {
  flex: 1;
  max-width: 48%;
}

.image-column img {
  width: 100%;
  height: auto;
  border-radius: 4px;
}

/* 响应式设计：在小屏幕上切换为垂直排列 */
@media screen and (max-width: 767px) {
  .image-row {
    flex-direction: column;
  }
  
  .image-column {
    max-width: 100%;
    margin-bottom: 15px;
  }
}
</style>