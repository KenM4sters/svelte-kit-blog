---
title: GAME_ENGINE MK2 OVERVIEW
description: A closer look at my 3D game engine written in C++ that exposes the Vulkan API
date: 2023-1-01
categories: 
    - Overview

published: true
---

**Game Engine - C++, Vulkan**
Unlike the predecessor to this project which was developed using C and the OpenGL API, this project takes advantage of the OOP paradigm to create a 3D game engine that comprises of several different systems that manage all the different aspects of a game that you can think of, from managing the entire graphics pipeline to processing user input. 

At the time of writing this, I’ve implemented several core systems that result in a 3D model being drawn to the screen that the user can pan around using the WASD and arrow keys. Besides the fundamentals, the project also uses some pretty cool performance enhancing techniques which, as the engine develops, will reduce CPU overhead and save memory on the GPU drastically.
 See below for a brief overview of a couple of those features:

    Staging Buffers - the most efficient type of memory for the GPU to read from usually isn’t accessible by the CPU, meaning that we would be unable to pass our vertex data into this storage buffer. The solution is therefore to create two buffers, one which can be read by the CPU and one that’s most efficient for the GPU to read from. We send our vertex data into the CPU-readable buffer (the staging buffer) and copy the data from that buffer to the GPU-efficient buffer. The advantage of this is that the GPU can process the vertex buffer quicker, and cases where the vertex buffer doesn’t need to be updated (or at least not regularly updated) the performance gain is worth it in large programs. If however, the vertex buffer needs to be updated very often, say for example if it contains colour data that changes over time, then the additional overhead of creating a staging buffer would likely counteract the benefits of increased read speed. 
    Push constants - the shader programs don’t have access to variables declared in our C++ program, but there’s a few ways that we can make them accessible. One very performant way is to use push constants, which are stored in buffers and pushed from the CPU to the GPU along with other command buffer data for use in shader modules. The most obvious drawback of using push constants is that they’re very limited in size, with 128 bytes being the maximum that the Vulkan API allows. Fortunately, this is more than enough for simple data like 3d/4d vectors and even a 4d matrix of floats (16 * 4 bytes = 64 bytes), making them an ideal candidate for transformation matrices like the model, view, projection or some other transformation matrix.
    I understood the complexity of creating a game engine from scratch before I embarked on this challenge, and even more so that over time, more and more studios will likely resort to using Epic’s open source Unreal Engine to reduce the overhead of maintaining such a complicated system, but understanding the fundamental concepts of a larger ideology is especially important to me, and I plan on continuing its development regardless of whether I end up working in engine development professionally or not. 
Ultimately, I’m eager to become proficient in using a robust game engine like Unreal, but also appreciate knowing what’s going on behind the scenes. 