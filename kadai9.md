# 課題９レポート

ORG = imread('Alps.jpg'); % 画像の読み込み  
ORG = rgb2gray(ORG); % 白黒濃淡画像に変換  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示

によって，原画像を読み込み，白黒濃淡画像に変換した結果を図１に示す．

![原画像](https://user-images.githubusercontent.com/56874442/71610241-a8013780-2bd2-11ea-9838-cbe5196388aa.png)
図1 白黒濃淡画像

ORG = imnoise(ORG,'salt & pepper',0.02); % ノイズ添付  
imagesc(ORG); colormap(gray); colorbar; % 画像の表示

![原画像](https://user-images.githubusercontent.com/56874442/71610215-72f4e500-2bd2-11ea-83a8-e5ad1ada2ad0.png)
図2 ノイズ添付画像

IMG = filter2(fspecial('average',3),ORG); % 平滑化フィルタで雑音除去  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示

![原画像](https://user-images.githubusercontent.com/56874442/71610299-252cac80-2bd3-11ea-8c50-fd541f3bd8f7.png)
図3 平滑化フィルタを通した画像

IMG = medfilt2(ORG,[3 3]); % メディアンフィルタで雑音除去  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示

![原画像](https://user-images.githubusercontent.com/56874442/71610378-b2700100-2bd3-11ea-9f52-a1b2bbcc8ddf.png)
図4 メディアンフィルタを通した画像

f=[0,-1,0;-1,5,-1;0,-1,0]; % フィルタの設計  
IMG = filter2(f,IMG,'same'); % フィルタの適用  
imagesc(IMG); colormap(gray); colorbar; % 画像の表示

![原画像](https://user-images.githubusercontent.com/56874442/71610414-2a3e2b80-2bd4-11ea-8f1f-269a653f5bc4.png)
図5 フィルタの適用画像
