# �ۑ�V���|�[�g

ORG = imread('Alps.jpg'); % �摜�̓ǂݍ���  
ORG = rgb2gray(ORG); % �����Z�W�摜�ɕϊ�  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��

�ɂ���āC���摜��ǂݍ��݁C�����Z�W�摜�ɕϊ��������ʂ�}�P�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/71598133-073a5a00-2b89-11ea-9853-d01fda891173.png)
�}1 �����Z�W�摜

imhist(ORG); % �Z�x�q�X�g�O�����𐶐��A�\��

![���摜](https://user-images.githubusercontent.com/56874442/71598233-5ed8c580-2b89-11ea-8c25-f4dcf6393fb3.png)
�}2 �Z�x�q�X�g�O����

% �_�C�i�~�b�N�����W��255�Ɋg��  
ORG = double(ORG);  
mn = min(ORG(:)); % �Z�x�l�̍ŏ��l���Z�o  
mx = max(ORG(:)); % �Z�x�l�̍ő�l���Z�o  
ORG = (ORG-mn)/(mx-mn) * 255;  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��

![���摜](https://user-images.githubusercontent.com/56874442/71598413-08b85200-2b8a-11ea-842c-66028654d9f1.png)
�}3 �_�C�i�~�b�N�����W255

ORG = uint8(ORG); % 8�r�b�g�ɕϊ�  
imhist(ORG); % �Z�x�q�X�g�O�����𐶐��A�\��

![���摜](https://user-images.githubusercontent.com/56874442/71599467-5c2c9f00-2b8e-11ea-97f3-bc4b577c1cc7.png)
�}3 �Z�x�q�X�g�O����
