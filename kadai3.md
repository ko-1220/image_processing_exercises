# 課題３レポート

ORG=imread('Alps.jpg'); % 原画像の入力  
ORG= rgb2gray(ORG); % カラー画像を白黒濃淡画像へ変換  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示

によって，原画像を読み込み，白黒濃淡画像に変換した結果を図１に示す．

![原画像](https://user-images.githubusercontent.com/56874442/71595118-cab53100-2b7d-11ea-892d-b049ca44f94a.png)  
図1 白黒濃淡画像

% 閾値64  
IMG = ORG > 64; % 輝度値が64以上の画素を1，その他を0に変換
imagesc(IMG); colormap(gray); colorbar;

![原画像](https://user-images.githubusercontent.com/56874442/71595363-98580380-2b7e-11ea-8b0e-fbcad5e7bdb1.png)  
図2 閾値64

% 閾値96  
IMG = ORG > 96;  
imagesc(IMG); colormap(gray); colorbar;

![原画像](https://user-images.githubusercontent.com/56874442/71595442-0dc3d400-2b7f-11ea-9569-802b5a74d947.png)  
図3 閾値96

% 閾値128  
IMG = ORG > 128;  
imagesc(IMG); colormap(gray); colorbar;

![原画像](https://user-images.githubusercontent.com/56874442/71595620-bc681480-2b7f-11ea-85d0-9cd7d68f4901.png)  
図4 閾値128

% 閾値192  
IMG = ORG > 192;  
imagesc(IMG); colormap(gray); colorbar;

![原画像](https://user-images.githubusercontent.com/56874442/71595702-110b8f80-2b80-11ea-9bbf-775aacac00b8.png)  
図5 閾値192
