---
title: "25-key MIDI keyboard"
excerpt: "A 25-key MIDI keyboard was designed and developed for use in both music games and music creation"
type: undergraduate
image: 2-cover.png
collection: projects
tags:
  - FPGA
  - Arduino
priority: 3
---

A 25-key MIDI keyboard was designed and developed for use in both music games and music creation. This keyboard can function both as a MIDI instrument featuring hundreds of timbres and as a control terminal for music games. 

In terms of technical implementation, the system utilizes an Arduino to convert hardware inputs into MIDI signal outputs according to the HCI protocol. Additionally, the project involved designing a music game mechanism and implemented this mechanism using an FPGA, along with the functionality to output real-time HDMI video animations during user interaction, to enhance the interactive experience.

<h3>Music Game Demo</h3>

<div class="video-container">
  <iframe src="//player.bilibili.com/player.html?bvid=BV1LDE1zDEy8&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>
</div>

<style>
.video-container {
  position: relative;
  padding-bottom: 56.25%; /* 16:9 比例 */
  height: 0;
  overflow: hidden;
  max-width: 100%;
  margin: 20px 0;
}

.video-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style> 