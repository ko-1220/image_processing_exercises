# �ۑ�S���|�[�g

ORG=imread('Alps.jpg'); % ���摜�̓���  
ORG=rgb2gray(ORG); % �J���[�摜�𔒍��Z�W�摜�֕ϊ�  
imagesc(ORG); colormap(gray); colorbar;

�ɂ���āC���摜��ǂݍ��݁C�����Z�W�摜�ɕϊ��������ʂ�}�P�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/71596248-25e92280-2b82-11ea-9038-f0523072f259.png)
�}1 �����Z�W�摜

% �q�X�g�O�����̕\��  
imhist(ORG);

![���摜](https://user-images.githubusercontent.com/56874442/71596643-72812d80-2b83-11ea-9ef5-1dedbc7523e0.png)
�}2 �q�X�g�O����
