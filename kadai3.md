# �ۑ�R���|�[�g

ORG=imread('Alps.jpg'); % ���摜�̓���  
ORG= rgb2gray(ORG); % �J���[�摜�𔒍��Z�W�摜�֕ϊ�  
imagesc(ORG); colormap(gray); colorbar; % �摜�̕\��

�ɂ���āC���摜��ǂݍ��݁C�����Z�W�摜�ɕϊ��������ʂ�}�P�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/71595118-cab53100-2b7d-11ea-892d-b049ca44f94a.png)  
�}1 �����Z�W�摜

% 臒l64  
IMG = ORG > 64; % �P�x�l��64�ȏ�̉�f��1�C���̑���0�ɕϊ�
imagesc(IMG); colormap(gray); colorbar;

![���摜](https://user-images.githubusercontent.com/56874442/71595363-98580380-2b7e-11ea-8b0e-fbcad5e7bdb1.png)  
�}2 臒l64

% 臒l96  
IMG = ORG > 96;  
imagesc(IMG); colormap(gray); colorbar;

![���摜](https://user-images.githubusercontent.com/56874442/71595442-0dc3d400-2b7f-11ea-9569-802b5a74d947.png)  
�}3 臒l96

% 臒l128  
IMG = ORG > 128;  
imagesc(IMG); colormap(gray); colorbar;

![���摜](https://user-images.githubusercontent.com/56874442/71595620-bc681480-2b7f-11ea-85d0-9cd7d68f4901.png)  
�}4 臒l128

% 臒l192  
IMG = ORG > 192;  
imagesc(IMG); colormap(gray); colorbar;

![���摜](https://user-images.githubusercontent.com/56874442/71595702-110b8f80-2b80-11ea-9bbf-775aacac00b8.png)  
�}5 臒l192
