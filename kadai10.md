# �ۑ�P�O���|�[�g

ORG = imread('Alps.jpg'); % ���摜�̓���  
ORG = rgb2gray(ORG); %�J���[����O���C�ւ̕ϊ�  
imagesc(ORG); colormap('gray'); colorbar;% �摜�\��

�ɂ���āC���摜��ǂݍ��݁C�����Z�W�摜�ɕϊ��������ʂ�}�P�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/71610519-2bbc2380-2bd5-11ea-9272-9312c3ab1037.png)
�}1 �����Z�W�摜

IMG = edge(ORG,'prewitt'); % �G�b�W���o�i�v���E�B�b�g�@�j  
imagesc(IMG); colormap('gray'); colorbar;% �摜�\��

![���摜](https://user-images.githubusercontent.com/56874442/71610567-79d12700-2bd5-11ea-82be-3dd0c46a2c25.png)
�}2 �v���E�B�b�g�@�ɂ��摜

IMG = edge(ORG,'sobel'); % �G�b�W���o�i�\�x���@�j  
imagesc(IMG); colormap('gray'); colorbar;% �摜�\��

![���摜](https://user-images.githubusercontent.com/56874442/71610629-eea46100-2bd5-11ea-877e-cfff6cf6b064.png)
�}3 �\�x���@�ɂ��摜

IMG = edge(ORG,'canny'); % �G�b�W���o�i�L���j�[�@�j  
imagesc(IMG); colormap('gray'); colorbar;% �摜�\��

![���摜](https://user-images.githubusercontent.com/56874442/71610654-3a570a80-2bd6-11ea-84a1-f4554e1fe6f5.png)
�}4 �L���j�[�@�ɂ��摜
