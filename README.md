# visualGrafic_repot
- 説明
  - 概要　 PCのカメラから動画を取得し、一定時間の間の画像の輝度値の平均をプロットする処理
  - 詳細
    - cv2.VIdeoCaptureで使用するデバイスのウインドウを開く。開けているかをcap.isOpenedで確認する。
    - While中cv2.imshow(~)で画像を連続して出力することで動画のようにしている。この画像の輝度の平均値を取得し配列に保存する
    - ｑを押すと、終了しplotする
    plotの処理はPlotDataで実装されており、生成した配列を引数に渡すとplotできる
- 使い方  
  -  上から順に実行してから、一番下を実行すると、カメラの画面が表示される。表示されない場合や別のカメラを使用したい時ははsave_frame_camera_keyの一つ目の引数に別の値を入れればよい  
  - ウインドウが表示されたらcを押すことでデータの取得が始まる。check　Endと表示された後qを押すとプロットされる


- 参考サイト
https://note.nkmk.me/python-opencv-camera-to-still-image/
カメラから画像を取得し動画のように表示する処理の参考にした

- 実行画像
![act](https://github.com/SaitoSeiji/visualGrafic_repot/blob/master/data/playImage.gif)
