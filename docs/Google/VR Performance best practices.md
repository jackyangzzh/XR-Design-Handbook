---
layout: default
title: VR Performance best practices
parent: Google
---

# VR Performance best practices
Original article: [VR Performance best practices](https://developers.google.com/vr/develop/best-practices/perf-best-practices)

## TL;DR
The article guides on optimizing mobile VR applications, addressing key bottlenecks like fill rate, draw calls, and thermal issues. It advises on managing CPU and GPU workloads, handling audio, UI, and garbage collection, and using techniques like multithreaded rendering and vertex processing. Recognizing and mitigating thermal loads on mobile devices are also vital to maintain performance and enhance user experience.

## Bullet points
1. 🎮 **Identifying bottlenecks** is crucial for optimizing your application performance. Both the CPU and GPU can contribute to these bottlenecks. Performance testing on both ends is vital to identify areas of your application that may be causing slower than desired operation.
   
2. 🖥️ **GPU optimization** often revolves around managing fill rate problems. These problems are typically related to the speed at which the GPU can fill the frame buffer, a storage area containing pixel data. The main factors include fragment shader processing, which computes the pixel's final color, and texture bandwidth, the rate at which textures can be mapped onto surfaces.
   
3. 📉 **Diagnosing fill rate problems** in mobile VR can be as straightforward as adjusting the resolution of your application. If the frame rate of your application increases when the resolution is lowered, it is a good indication that your application is experiencing fill rate issues. 
   
4. 🛠️ **Solutions to fix fill rate issues** vary, but they often include adjusting post-process effects that can be GPU-intensive, managing render target bandwidth to reduce the amount of data sent to the GPU, and optimizing texture bandwidth use by compressing textures or using mipmaps, for example.
   
5. 💡 **CPU optimization** often involves the efficient management of tasks such as draw calls, which are commands to the GPU to render objects, audio processing, physics simulations, custom scripts, UI updates, and garbage collection (automatic memory management) in Unity. These tasks can strain the CPU if not properly optimized.
   
6. 🔊 **Audio processing** can be optimized by reducing the sampling rate (the number of times per second audio is sampled), limiting the number of audio clips being played simultaneously, and using hardware decompression for audio sources, which uses the device's hardware to decompress audio data, reducing CPU usage.
   
7. 🎨 **Draw calls** can cause CPU bottlenecks if too many objects are being rendered in a single frame. Techniques to reduce this cost can include using multithreaded rendering, which allows draw calls to be processed on multiple CPU cores, or reducing the number of draw calls by merging similar objects into a single mesh, for example.
   
8. 👾 **GPU vertex processing optimization** can improve frame rates. The vertex processing stage of the rendering pipeline involves transforming the vertices of a 3D model and calculating their lighting. By adding geometric detail to a 3D model, it's possible to reduce the need for a normal map (a texture that adds detail to a surface) or additional texture lookups, thereby potentially improving frame rate.
   
9.  🗑️ **Effective garbage collection** in Unity can contribute to maintaining a smooth frame rate in VR applications. Garbage collection is the automatic reclamation of memory that is no longer in use by the program. By avoiding per-frame memory allocations and creating all necessary objects at the beginning of your game, you can minimize the impact of garbage collection on your frame rate.
    
10. 🌡️ **Thermal issues** can cause significant performance drops after extended use of a mobile VR application. It is important to monitor Android device logs for signs of thermal throttling, a phenomenon where the device reduces its performance to cool down. Keeping track of the device temperature and managing the thermal loads effectively is essential to prevent overheating and ensure consistent performance.

## Keywords
- **Bottlenecks**: These refer to the specific parts of a system that limit the overall performance. In the context of the transcription, it applies to elements in the application that reduce its operational speed.

- **CPU (Central Processing Unit)**: The primary component of a computer that performs most of the processing. In gaming applications, it's responsible for tasks like draw calls, physics simulations, audio processing, UI updates, and memory management.

- **GPU (Graphics Processing Unit)**: A specialized processor designed to accelerate graphics rendering. In gaming applications, the GPU handles tasks like fragment shader processing and texture mapping.

- **Fill Rate**: The speed at which the GPU can fill the frame buffer, or in other words, render and display frames on the screen. Fill rate issues can reduce the frame rate of an application.

- **Fragment Shader**: A type of shader in graphics used to compute the final color of a pixel. They can contribute to fill rate problems if not properly optimized.

- **Render Target Bandwidth**: The rate at which data is sent to the GPU for rendering. Optimizing the render target bandwidth can help improve GPU performance.

- **Draw Calls**: Commands sent to the GPU to render objects. If not efficiently managed, draw calls can strain the CPU and reduce the performance of an application.

- **Audio Processing**: The task of generating and managing sounds within an application. Efficient audio processing involves reducing CPU usage while maintaining good sound quality.

- **Multithreaded Rendering**: A technique that allows draw calls to be processed on multiple CPU cores, thereby improving the performance of an application.

- **GPU Vertex Processing**: A stage in the GPU rendering pipeline that involves transforming the vertices of a 3D model and calculating their lighting. Optimizing vertex processing can improve frame rates.

- **Garbage Collection**: An automatic memory management system that reclaims memory no longer in use by the program. Effective garbage collection in VR applications can contribute to maintaining a smooth frame rate.

- **Thermal Throttling**: A phenomenon where a device reduces its performance to cool down. It's essential to manage thermal loads effectively to prevent overheating and ensure consistent performance in mobile VR applications.
