# Residual U-Net for Semantic Segmentation

## 概要
本プロジェクトでは、U-NetのEncoderにResidual Blockを導入し、セマンティックセグメンテーションの精度向上を試みた。既存のU-Net構造を維持しつつ、特徴抽出能力と学習の安定性を改善したモデルを構築した。検証データではmIoU 0.8956を達成し、Residual接続による表現力向上の有効性を確認した。

## 背景
U-Netは画像セグメンテーションにおいて広く用いられるモデルであるが、深層化に伴う特徴の劣化や学習の不安定性が課題となる。そのため、本プロジェクトではResidual Blockを導入し、これらの課題の改善を目指した。

## モデル構成
- Encoder：Residual Blockによる特徴抽出
- Decoder：空間解像度復元
- Skip Connection：空間情報の保持

## 成果
- mIoU：0.8956

## 技術スタック
- Python
- PyTorch
- Deep Learning（U-Net, Residual Network）
- Image Segmentation

## 工夫点
Encoder部分をResidual Blockに置き換えることで、深い層でも特徴伝播が可能となり、モデルの学習安定性と表現力の向上を実現した。

## 詳細
詳細な実装および評価については以下のPDFを参照してください
- Semantic_Segmentation.pdf
