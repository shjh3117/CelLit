# **Custom CelLit Shader for Unreal Engine 5**
![image](https://github.com/user-attachments/assets/65949c17-e43f-42b8-9bb8-a68128da509d)

**CelLit** is a **cel-shading style lighting shader** implemented in Unreal Engine 5.

## View in Other Languages
- [English](README.md)
- [한국어](README.ko.md)
- [日本語](README.ja.md)

## Introduction
This shader applies lighting effects in the style of manga or animation.  
It modifies the HLSL code of the engine's subsurface shading model, requiring the engine's shader files to be replaced.

CelLit Shader offers the following key features:

- **Cel Lit**  
  Cartoon-like representation for surfaces receiving direct light (Two-tone shading).  
  Supports all types of lighting.  
  Suppresses self-shadowing.  
  
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
- **Key Supported Technologies**  
  Lumen (Supports both HW/SW ray tracing)  
  VSM (Virtual Shadow Maps)  
  
- **Incompatible Technologies**  
  SM5 and below  
  Mobile Shader  
  Ray tracing Shadows  
  
## Installation Instructions
1. Copy `/Engine/Renderer/...` to your engine directory.
