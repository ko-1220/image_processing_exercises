# �ۑ�U���|�[�g

ORG=imread('Alps.jpg'); % ���摜�̓���  
ORG = rgb2gray(ORG);  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��

�ɂ���āC���摜��ǂݍ��݁C�����Z�W�摜�ɕϊ��������ʂ�}�P�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/71597578-1f10de80-2b87-11ea-9b77-357234bbe366.png)
�}1 �����Z�W�摜

IMG = ORG>128; % 臒l128�ɂ���l��  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��

![���摜](https://user-images.githubusercontent.com/56874442/71597696-99d9f980-2b87-11ea-9128-6fe7dc53518d.png)
�}2 臒l128�ɂ���l���摜

IMG = dither(ORG); % �f�B�U�@�ɂ���l��  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��

![���摜](https://user-images.githubusercontent.com/56874442/71597811-f76e4600-2b87-11ea-94de-4f64f7784cc2.png)
�}3 �f�B�U�@�ɂ���l���摜
