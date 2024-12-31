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


- **Cel Lit**  
  ![ScreenRecording2024-12-31123447-ezgif com-resize](https://github.com/user-attachments/assets/ab3b5d02-efdb-4592-93e4-8cfe7a61b9b7)  
  Cartoon-like representation for surfaces receiving direct light (Two-tone shading).  
  Supports all types of lighting.  
  Supports Saturate/Value shift in two tone.  
  Suppresses self-shadowing.  
  Compatible with PBR  
  
- **Cel Global Illumination**  
  ![20241231-0422-08 2373269-ezgif com-resize](https://github.com/user-attachments/assets/39da4092-d2cb-4790-83d0-4513dff94a0e)  
  Cartoon-like representation for surfaces not directly lit (Multiple-tone shading).  
  Compatible with Lumen indirect lighting.  
  
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

## Technical Features  
- **Support**  
  Lumen (Supports both HW/SW ray tracing)  
  Virtual shadow maps  
  Physically based rendering  
  
- **Incompatible**  
  SM5 and below  
  Mobile Shader  
  Ray traced shadow
  
## Installation Instructions
1. Copy `/Engine/Shaders/...` to your engine directory.
2. Run engine.
Not require engine build!!
