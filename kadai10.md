# 課題１０レポート

ORG = imread('Alps.jpg'); % 原画像の入力  
ORG = rgb2gray(ORG); %カラーからグレイへの変換  
imagesc(ORG); colormap('gray'); colorbar;% 画像表示

によって，原画像を読み込み，白黒濃淡画像に変換した結果を図１に示す．

![原画像](https://user-images.githubusercontent.com/56874442/71610519-2bbc2380-2bd5-11ea-9272-9312c3ab1037.png)
図1 白黒濃淡画像

IMG = edge(ORG,'prewitt'); % エッジ抽出（プレウィット法）  
imagesc(IMG); colormap('gray'); colorbar;% 画像表示

![原画像](https://user-images.githubusercontent.com/56874442/71610567-79d12700-2bd5-11ea-82be-3dd0c46a2c25.png)
図2 プレウィット法による画像

IMG = edge(ORG,'sobel'); % エッジ抽出（ソベル法）  
imagesc(IMG); colormap('gray'); colorbar;% 画像表示

![原画像](https://user-images.githubusercontent.com/56874442/71610629-eea46100-2bd5-11ea-877e-cfff6cf6b064.png)
図3 ソベル法による画像

IMG = edge(ORG,'canny'); % エッジ抽出（キャニー法）  
imagesc(IMG); colormap('gray'); colorbar;% 画像表示

![原画像](https://user-images.githubusercontent.com/56874442/71610654-3a570a80-2bd6-11ea-84a1-f4554e1fe6f5.png)
図4 キャニー法による画像
