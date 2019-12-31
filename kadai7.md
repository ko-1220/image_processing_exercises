# 課題７レポート

ORG = imread('Alps.jpg'); % 画像の読み込み  
ORG = rgb2gray(ORG); % 白黒濃淡画像に変換  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示

によって，原画像を読み込み，白黒濃淡画像に変換した結果を図１に示す．

![原画像](https://user-images.githubusercontent.com/56874442/71598133-073a5a00-2b89-11ea-9853-d01fda891173.png)
図1 白黒濃淡画像

imhist(ORG); % 濃度ヒストグラムを生成、表示

![原画像](https://user-images.githubusercontent.com/56874442/71598233-5ed8c580-2b89-11ea-8c25-f4dcf6393fb3.png)
図2 濃度ヒストグラム

% ダイナミックレンジを255に拡大  
ORG = double(ORG);  
mn = min(ORG(:)); % 濃度値の最小値を算出  
mx = max(ORG(:)); % 濃度値の最大値を算出  
ORG = (ORG-mn)/(mx-mn) * 255;  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示

![原画像](https://user-images.githubusercontent.com/56874442/71598413-08b85200-2b8a-11ea-842c-66028654d9f1.png)
図3 ダイナミックレンジ255

ORG = uint8(ORG); % 8ビットに変換  
imhist(ORG); % 濃度ヒストグラムを生成、表示

![原画像](https://user-images.githubusercontent.com/56874442/71599467-5c2c9f00-2b8e-11ea-97f3-bc4b577c1cc7.png)
図3 濃度ヒストグラム
