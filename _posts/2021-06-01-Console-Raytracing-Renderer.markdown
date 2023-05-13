---
layout: default
title: Console Raytracing Renderer
modal-id: 2
date: 2021-06-01
imgThumbnail: ConsoleRaytracer/ConsoleRaytracerThumbnail.png
img:
    - active: true
      video: "ConsoleRaytracer/F_CurrentResult.mp4"
    - video: "ConsoleRaytracer/E_RGBCirclesWithBugLines.mp4"
    - video: "ConsoleRaytracer/D_AnsiCircles.mp4"
    - video: "ConsoleRaytracer/C_ASCIISpheresGPU.mp4"
    - video: "ConsoleRaytracer/B_ASCIIShapes.mp4"
    - video: "ConsoleRaytracer/A_ASCII3DWithoutShading.mp4"
alt: image-alt
project-date: 2021-2023
category: Hobby project - 3D Rendering
description: 
    - This is a hobby project that I have worked on a bit the last three years. My initial goal with the project was to see how far I could get with a raytracing implementation while using as few libraries as possible, working in only C++ and CUDA.
    - The pictures above show the progress, starting at the current state of the project, and going backwards to earlier iterations.
    - All rendering is done within the Windows console. With the "pixels" being a two-dimensional array of colored characters that is printed to the console. The raytracing is done using CUDA, essentially creating a pixelshader on the GPU. Although, neither DirectX, OpenGL, nor Vulkan are used in this project. In the pixel shader the ASCII characters are assigned to the pixels, depending on shading value and if the renderer is currently in ASCII mode.
    - All spheres and shapes that are visible are being updated on the GPU. This in conjunction with my own implementation of a type of bounding volume hierarchy on the GPU means negligible impact on performance as more and more objects are introduced in the scene.
    - The largest bottleneck to the performance of the project is the printing of the console, which is out of my hands. I moved the printing to the console to a seperate CPU thread and implemented my own swapchain to increase print-performance, but nonetheless the printer thread sometimes is around 30 FPS, depending on how much is seen on the screen, while the rendering thread comfortably stays above 180 FPS with over 300 spheres in the scene.
    - Because of this restriction, I have started a 2nd version of this project, which will use SDL for window management instead of the Windows console.
languages: C++, CUDA
github: https://github.com/EmilHogstedt/Raytracing-in-Windows-Console
---
