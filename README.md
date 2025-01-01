# **Custom cel-shading style shader for Unreal Engine 5**
![Screenshot2024-12-29205635-ezgif com-resize](https://github.com/user-attachments/assets/a1398d67-b2ad-4e15-828d-f196b49f4528)

**CelLit** is a **cel-shading style shader** implemented in Unreal Engine 5.

## View in Other Languages
- [English](README.md)
- [한국어](README.ko.md)
- [日本語](README.ja.md)

## Introduction
This shader applies lighting effects in the style of manga or animation.  
It modifies the HLSL code of the engine's subsurface shading model, requiring the engine's shader files to be replaced.

CelLit Shader offers the following key features:

- **Cel Lit Rendering**  
  ![ScreenRecording2024-12-31123447-ezgif com-resize](https://github.com/user-attachments/assets/ab3b5d02-efdb-4592-93e4-8cfe7a61b9b7)  
  Cartoon-like shading for surfaces lit by direct lighting (Two-tone shading).  
  Supports all types of lighting.  
  Supports Saturate/Value shift in two tone.  
  Suppresses self-shadowing.  
  Compatible with PBR  

- **Cel Global Illumination Rendering**  
  ![20241231-0422-08 2373269-ezgif com-resize](https://github.com/user-attachments/assets/39da4092-d2cb-4790-83d0-4513dff94a0e) ![Screenshot2024-12-31153322-ezgif com-resize](https://github.com/user-attachments/assets/a2db7a80-8c63-4d67-89cb-20a9abf210af) ![Screenshot2025-01-01172558-ezgif com-resize](https://github.com/user-attachments/assets/fe3abbf7-48d6-44dc-9cdf-693a3e9100b8)  

  Cartoon-like shading for surfaces lit by indirect lighting (multi-tone shading).  
  Compatible with Lumen indirect lighting (Ex. Lit by Emissive Color).  
  Noise Attenuation through Low-Frequency Filtering.  
  
- **Cel Face Shadow**  
  ![CelLitSampleProject - 언리얼 에디터 12_31_2024 1_34_52 PM](https://github.com/user-attachments/assets/089071c0-1e65-481f-b8dd-f556802f4125)  
  Cartoon-like facial shading for surfaces receiving direct light.  
  Supports face shadow maps.
  
- **OutLine**  
  Provides a post-process material using Sobel filtering for edge detection.  
  Includes multiple customizable parameters.  
  Specialized outline detection for hair.  

- **2D Shadow**  
  Supports 2D shadows specifically for hair.  

## Specification
- **Supported Features**  
  Lumen (supports both hardware and software ray tracing)  
  Virtual shadow maps (VSM)  
  Physically Based Rendering (PBR)  
    
- **Incompatible Features**  
  Shader Model 5 (SM5) and below  
  Mobile
  Ray traced shadows  
  
## Installation Instructions
1. Copy `/Engine/Shaders/...` to your engine directory.
2. Run sample porject.
No engine build required!
