# 課題６レポート

ORG=imread('Alps.jpg'); % 原画像の入力  
ORG = rgb2gray(ORG);  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示

によって，原画像を読み込み，白黒濃淡画像に変換した結果を図１に示す．

![原画像](https://user-images.githubusercontent.com/56874442/71597578-1f10de80-2b87-11ea-9b77-357234bbe366.png)
図1 白黒濃淡画像

IMG = ORG>128; % 閾値128による二値化  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示

![原画像](https://user-images.githubusercontent.com/56874442/71597696-99d9f980-2b87-11ea-9128-6fe7dc53518d.png)
図2 閾値128による二値化画像

IMG = dither(ORG); % ディザ法による二値化  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示

![原画像](https://user-images.githubusercontent.com/56874442/71597811-f76e4600-2b87-11ea-94de-4f64f7784cc2.png)
図3 ディザ法による二値化画像
