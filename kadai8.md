# �ۑ�W���|�[�g

ORG = imread('Alps.jpg'); % �摜�̓ǂݍ���  
ORG = rgb2gray(ORG); % �����Z�W�摜�ɕϊ�  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��

�ɂ���āC���摜��ǂݍ��݁C�����Z�W�摜�ɕϊ��������ʂ�}�P�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/71609971-37591b80-2bd0-11ea-95fd-da9b2f3f1c16.png)
�}1 �����Z�W�摜

IMG = ORG > 128; % 臒l128�œ�l��  
imagesc(IMG); colormap(gray); colorbar; % �摜�̕\��

![���摜](https://user-images.githubusercontent.com/56874442/71610020-c1a17f80-2bd0-11ea-8356-cd63414a5f90.png)
�}2 臒l128�̓�l�摜

% ���x�����O  
IMG = bwlabeln(IMG);  
imagesc(IMG); colormap(jet); colorbar; % �摜�̕\��

![���摜](https://user-images.githubusercontent.com/56874442/71610072-468c9900-2bd1-11ea-897a-9d0e83fc44cd.png)
