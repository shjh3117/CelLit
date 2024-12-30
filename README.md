# **Custom CelLit Shader for Unreal Engine 5**
![image](https://github.com/user-attachments/assets/65949c17-e43f-42b8-9bb8-a68128da509d)

**CelLit**은 Unreal Engine 5에서 구현된 **셀 셰이딩 스타일 조명 쉐이더**입니다.
---

## **소개**
만화나 애니메이션 스타일의 조명 효과를 적용할 수 있습니다.  
엔진의 Subsurface shading model의 hlsl 코드 수정을 통해 구현되었기에 엔진의 쉐이더를 파일을 교체하여야 합니다.  

CelLit Shader는 다음과 같은 주요 특징을 제공합니다.
- **Cel Lit**  
  조명을 받는 표면에 대한 만화 같은 표현. (Two tone)  
  모든 종류의 조명에 대응.  
  Self-Shadow 억제.
  
- **Cel Global Illumination**  
  조명을 받지 않는 표면에 대한 만화 같은 표현. (Multiple Tone).  
  Lumen 간접광 대응.
  
- **Cel Face Sadow**  
  조명을 받는 표면에 대한 만화 같은 얼굴 표현.
  
- **OutLine**  
  Sobel Filltering에 의한 아웃라인 검출 PostProcess Material 제공.
  여러 파라미터 제공.  
  머리카락 특화 아웃라인 검출 제공.  
---

## **설치 방법**
1. Copy /Engine/Renderer/... to your engine directory.
