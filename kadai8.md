# 課題８レポート

ORG = imread('Alps.jpg'); % 画像の読み込み  
ORG = rgb2gray(ORG); % 白黒濃淡画像に変換  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示

によって，原画像を読み込み，白黒濃淡画像に変換した結果を図１に示す．

![原画像](https://user-images.githubusercontent.com/56874442/71609971-37591b80-2bd0-11ea-95fd-da9b2f3f1c16.png)
図1 白黒濃淡画像

IMG = ORG > 128; % 閾値128で二値化  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示

![原画像](https://user-images.githubusercontent.com/56874442/71610020-c1a17f80-2bd0-11ea-8356-cd63414a5f90.png)
図2 閾値128の二値画像

% ラベリング  
IMG = bwlabeln(IMG);  
imagesc(IMG); colormap(jet); colorbar; % 画像の表示

![原画像](https://user-images.githubusercontent.com/56874442/71610072-468c9900-2bd1-11ea-897a-9d0e83fc44cd.png)
