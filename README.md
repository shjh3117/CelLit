# Test branch  

# **Custom cel-shading style shader for Unreal Engine 5**
![Screenshot2024-12-29205635-ezgif com-resize](https://github.com/user-attachments/assets/a1398d67-b2ad-4e15-828d-f196b49f4528)

**CelLit** is a **cel-shading style shader** implemented in Unreal Engine 5.

## View in Other Languages
- [English](README.md)
- [한국어](README.ko.md)

## Introduction
This shader applies lighting effects in the cartoon of manga or animation.  
It modifies the HLSL code of the engine's preintergrated skin shading model and cloth shading model, so requiring the engine's shader files to be replaced.  
CelLit Shader offers the following key features:   

- **Cel Rendering**  
  ![20250213-1750-15 2693118-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/3ac52842-b305-437c-bc2d-e830d6c6a541) ![image-ezgif com-resize](https://github.com/user-attachments/assets/5619a1aa-3b7e-4d6c-b600-0a16f2385a36)  
  Cartoon-like shading for surfaces lit by direct lighting.  
  Supports Mult-tone Shading(2-10 tone).  
  Supports Shadow threshold map.  
  Suppresses self-shadowing.  
  Compatible with all types of lighting.  
  Compatible with transmission.  
  Compatible with PBR,  

- **Cel Global Illumination Rendering**  
  ![20241231-0422-08 2373269-ezgif com-resize](https://github.com/user-attachments/assets/39da4092-d2cb-4790-83d0-4513dff94a0e) ![Screenshot2024-12-31153322-ezgif com-resize](https://github.com/user-attachments/assets/a2db7a80-8c63-4d67-89cb-20a9abf210af) ![Screenshot2025-01-01172558-ezgif com-resize](https://github.com/user-attachments/assets/fe3abbf7-48d6-44dc-9cdf-693a3e9100b8)  

  Cartoon-like shading for surfaces lit by indirect lighting (multi-tone shading).  
  Compatible with Lumen indirect lighting (Ex. Lit by Emissive Color).  
  Noise Attenuation through Low-Frequency Filtering.  
  
- **OutLine**  
  Provides a post-process material using Sobel filtering for edge detection.  
  Includes multiple customizable parameters.  
  Specialized outline detection for hair.  

## Specification
- **Compatible Features**  
  Lumen (supports both hardware and software ray tracing)  
  Virtual shadow maps (VSM)  
  Physically Based Rendering (PBR)  
    
- **Incompatible Features**  
  Shader Model 5 (SM5) and below  
  Mobile
  Ray traced shadows  
  
## Installation Instructions
1. Copy `/Engine/Shaders/...` to your engine directory. (https://github.com/shjh3117/UnrealEngine_test) ([404error](https://forums.unrealengine.com/t/getting-error-404-in-github-while-trying-do-access-the-unreal-engine-source-code-repository/1312189)
2. Run sample porject.
No engine build required!

## Usage
  Cloth Shading Model is a normal CelLit Material.  
  Preintergrated skin Shading Model is for face shading.
