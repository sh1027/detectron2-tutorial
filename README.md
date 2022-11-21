# detectron2_tutorial

事前学習済みモデル(model_zoo)による推論を試すチュートリアルコード

AIコンソーシアムの講義 (2022年 物体検出入門) で使用

### チュートリアルの内容

#### 推論対象

- COCOデータセットの画像
- Google Drive内の画像
- Google Drive内の動画
- YouTubeの動画

#### タスク

- Object detection 
- Instance segmentation 
- Keypoint detection 
- Panoptic segmentation

### 公式チュートリアルからの主な変更点

- 複数タスクの推論コードを`Detector`クラスに集約 → 手軽にタスクを切り替え可能
- Google Drive内のファイルに対する推論
- 動画のダウンロードに用いるライブラリの変更 (`youtube-dl`から`yt-dlp`へ) → 処理速度アップ
- 動画の推論結果をcolab上で再生できるように変更
- プチ演習の追加
  - 推論結果のフィルタリング
  - セグメンテーションを利用した画像編集
  
