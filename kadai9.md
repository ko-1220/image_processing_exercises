# �ۑ�X���|�[�g

ORG = imread('Alps.jpg'); % �摜�̓ǂݍ���  
ORG = rgb2gray(ORG); % �����Z�W�摜�ɕϊ�  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��

�ɂ���āC���摜��ǂݍ��݁C�����Z�W�摜�ɕϊ��������ʂ�}�P�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/71610241-a8013780-2bd2-11ea-9838-cbe5196388aa.png)
�}1 �����Z�W�摜

ORG = imnoise(ORG,'salt & pepper',0.02); % �m�C�Y�Y�t  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��

![���摜](https://user-images.githubusercontent.com/56874442/71610215-72f4e500-2bd2-11ea-83a8-e5ad1ada2ad0.png)
�}2 �m�C�Y�Y�t�摜

IMG = filter2(fspecial('average',3),ORG); % �������t�B���^�ŎG������  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��

![���摜](https://user-images.githubusercontent.com/56874442/71610299-252cac80-2bd3-11ea-8c50-fd541f3bd8f7.png)
�}3 �������t�B���^��ʂ����摜

IMG = medfilt2(ORG,[3 3]); % ���f�B�A���t�B���^�ŎG������  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��

![���摜](https://user-images.githubusercontent.com/56874442/71610378-b2700100-2bd3-11ea-9f52-a1b2bbcc8ddf.png)
�}4 ���f�B�A���t�B���^��ʂ����摜

f=[0,-1,0;-1,5,-1;0,-1,0]; % �t�B���^�̐݌v  
IMG = filter2(f,IMG,'same'); % �t�B���^�̓K�p  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��

![���摜](https://user-images.githubusercontent.com/56874442/71610414-2a3e2b80-2bd4-11ea-8f1f-269a653f5bc4.png)
�}5 �t�B���^�̓K�p�摜
