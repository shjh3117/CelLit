# **Custom cel-shading style shader for Unreal Engine 5**
![image](https://github.com/user-attachments/assets/65949c17-e43f-42b8-9bb8-a68128da509d)

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
  ![ScreenRecording2024-12-31123447-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/4b4ec8b3-3335-4cdc-9743-0a6c60a53409)  
  Cartoon-like representation for surfaces receiving direct light (Two-tone shading).  
  Supports all types of lighting.  
  Suppresses self-shadowing.  
  compatible PBR  
  
- **Cel Global Illumination**  
  Cartoon-like representation for surfaces not directly lit (Multiple-tone shading).  
  Compatible with Lumen indirect lighting.  
  
- **Cel Face Shadow**  
  Cartoon-like facial shading for surfaces receiving direct light.  
  Supports face shadow maps.  
  
- **OutLine**  
  Provides a post-process material using Sobel filtering for edge detection.  
  Includes multiple customizable parameters.  
  Specialized outline detection for hair.  

- **2D Shadow**  
  Supports 2D shadows specifically for hair.  

## Technical Features  
- **Supported Features**  
  Lumen (Supports both HW/SW ray tracing)  
  VSM (Virtual Shadow Maps)  
  
- **Incompatible Features**  
  SM5 and below  
  Mobile Shader  
  Ray traced shadow
  
## Installation Instructions
1. Copy `/Engine/Shaders/...` to your engine directory.
