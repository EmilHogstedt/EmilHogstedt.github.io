---
layout: default
title: DirectX12 Project
modal-id: 4
date: 2020-01-01
imgThumbnail: DirectX12Project/Thumbnail.png
img:
    - active: true
      link: "DirectX12Project/Comparison.png"
    - video: "DirectX12Project/video.mp4"
alt: image-alt
project-date: Q2 2022
category: Course project - 3D Programming with DirectX12
description: 
    - Me and one other student made this project for our DirectX12 course, where we were allowed to choose different 3D Programming techniques to implement using DirectX12. The three techniques we decided to implement were; Vertex Pulling, Frames in Flight, and Inlined Ray Tracing using DirectX Ray Tracing (DXR) 1.1. My chosen technique and responsibility was the Inlined Ray Tracing.
    - My implementation of Inlined Ray Tracing was used to produce the shadows that can be seen in the picture and video above. The picture shows a side-by-side comparison of the result with and without the technique.
    - To be able to perform Inlined Ray Tracing in the shaders using HLSL the Ray Tracing Acceleration structures first need to be set up on the CPU, which is the bulk of the time spent implementing this technique. Essentially these hold the data of the objects that are to be traced in the shader.
    - Our report can be found by pressing the Chrome-icon below.
languages: C++ - DirectX12 - HLSL
github: https://github.com/EmilHogstedt/DirectX12Project
chrome: "..\DirectX12Report.pdf"
---
