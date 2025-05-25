---
title: "SmartGuide: An Immersive Location-based Tour Guide Platform for Smart Glasses"
excerpt: "An immersive, location-based tour guide platform developed for smart glasses users"
type: undergraduate
image: 1-cover.png
collection: projects
tags:
  - Wearable Devices
  - Unity
  - App Development
priority: 2
---

SmartGuide is an immersive, location-based tour guide platform developed for smart glasses users. Its core functionality allows users to upload and receive location-bound audio messages at specific places, thereby sharing personal experiences, digitizing memories, and offering unique perspectives to subsequent visitors. The platform also provides route recommendation and navigation features, helping users explore destinations more efficiently.

In terms of technical implementation, the smart glasses client utilizes the MVP (Model-View-Presenter) architecture, leveraging gyroscope and accelerometer data for pose estimation and voice-assisted positioning. The software application is developed with Unity3D, integrating Mapbox for precise location tracking and map generation, and includes features such as text-to-speech and navigation path planning. 

<div class="image-row">
  <div class="image-column">
    <img src="../../images/projects/undergraduate/page1.png" alt="图片1描述">
  </div>
  <div class="image-column">
    <img src="../../images/projects/undergraduate/page2.png" alt="图片2描述">
  </div>
</div>

<style>
.image-row {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin: 20px 0;
  max-width: 80%;
  margin-left: auto;
  margin-right: auto;
}

.image-column {
  flex: 1;
  max-width: 45%;
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
    max-width: 90%;
  }
  
  .image-column {
    max-width: 100%;
    margin-bottom: 15px;
  }
}
</style>
