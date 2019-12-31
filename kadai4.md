# 課題４レポート

ORG=imread('Alps.jpg'); % 原画像の入力  
ORG=rgb2gray(ORG); % カラー画像を白黒濃淡画像へ変換  
imagesc(ORG); colormap(gray); colorbar;

によって，原画像を読み込み，白黒濃淡画像に変換した結果を図１に示す．

![原画像](https://user-images.githubusercontent.com/56874442/71596248-25e92280-2b82-11ea-9038-f0523072f259.png)
図1 白黒濃淡画像

% ヒストグラムの表示  
imhist(ORG);

![原画像](https://user-images.githubusercontent.com/56874442/71596643-72812d80-2b83-11ea-9ef5-1dedbc7523e0.png)
図2 ヒストグラム
