# **Custom cel-shading style shader for Unreal Engine 5**
![image](https://github.com/user-attachments/assets/65949c17-e43f-42b8-9bb8-a68128da509d)

**CelLit**はUnreal Engine 5で実装された**セルシェーディングスタイルのライティングシェーダー**です。

## 他の言語で見る
- [English](README.md)
- [한국어](README.ko.md)
- [日本語](README.ja.md)

## 紹介
マンガやアニメーションのスタイルのライティング効果を適用できます。  
エンジンのSubsurface shading modelのHLSLコードを修正することで実装されているため、エンジンのシェーダーファイルを置き換える必要があります。

CelLit Shaderは以下のような主要な特徴を提供します。
- **Cel Lit**  
  ライティングを受ける表面に対するマンガのような表現（ツートーンシェーディング）。  
  すべての種類のライティングに対応。  
  セルフシャドウの抑制。  
  
- **Cel Global Illumination**  
  直接的にライティングを受けない表面に対するマンガのような表現（マルチトーンシェーディング）。  
  Lumenの間接光に対応。  
  
- **Cel Face Shadow**  
  ライティングを受ける表面に対するマンガのような顔の表現。  
  Face Shadow Mapをサポート。  
  
- **OutLine**  
  Sobelフィルタリングを使用して検出するPostProcessマテリアルを提供。  
  複数のパラメータを提供。  
  髪の毛特化のアウトライン検出を提供。  

- **2D Shadow**  
  髪の毛に対する2Dシャドウをサポート。  

## 技術的特徴  
- **主要なサポート機能**  
  Lumen（HW/SWレイトレーシング両方をサポート）  
  VSM（バーチャルシャドウマップ）  
  
- **非互換機能**  
  SM5およびそれ以前  
  モバイルシェーダー  
  レイトレースシャドウ
  
## インストール方法
1. `/Engine/Renderer/...` をエンジンディレクトリにコピーします。
