# �ۑ�P���|�[�g

�W���摜�uAlps�v�����摜�Ƃ���D���̉摜�͏c512�摜�C��512��f�ɂ�鐳���`�̃f�B�W�^���J���[�摜�ł���D

ORG=imread('Alps.jpg'); % ���摜�̓���  
imagesc(ORG); axis image; % �摜�̕\��

�ɂ���āC���摜��ǂݍ��݁C�\���������ʂ�}�P�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/69960565-1bb91180-154d-11ea-9e2a-07be9917711c.png)
�}1 ���摜

���摜��1/2�T���v�����O����ɂ́C�摜��1/2�{�ɏk��������C2�{�Ɋg�傷��΂悢�D�Ȃ��C�g�傷��ۂɂ́C�P����Ԃ��邽�߂Ɂubox�v�I�v�V������ݒ肷��D

IMG = imresize(ORG,0.5); % �摜�̏k��  
IMG2 = imresize(IMG,2,'box'); % �摜�̊g��

1/2�T���v�����O�̌��ʂ�}�Q�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/69975768-271b3580-156b-11ea-9ada-51b39b442140.png)  
�}2 1/2�T���v�����O

���l�Ɍ��摜��1/4�T���v�����O����ɂ́C�摜��1/2�{�ɏk��������C2�{�Ɋg�傷��΂悢�D���Ȃ킿�C

IMG = imresize(ORG,0.5); % �摜�̏k��  
IMG2 = imresize(IMG,2,'box'); % �摜�̊g��

�Ƃ���D1/4�T���v�����O�̌��ʂ�}�R�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/69975839-4fa32f80-156b-11ea-8da4-aedd57ca8b44.png)  
�}3 1/4�T���v�����O

1/8����1/32�T���v�����O�́C

IMG = imresize(ORG,0.5); % �摜�̏k��  
IMG2 = imresize(IMG,2,'box'); % �摜�̊g��

���J��Ԃ��D�T���v�����O�̌��ʂ�}�S�`�U�Ɏ����D

![���摜](https://user-images.githubusercontent.com/56874442/69975900-6cd7fe00-156b-11ea-9f99-861b6a2de326.png)  
�}4 1/8�T���v�����O

![���摜](https://user-images.githubusercontent.com/56874442/69975951-89743600-156b-11ea-8ccb-910dc3e957a5.png)  
�}5 1/16�T���v�����O

![���摜](https://user-images.githubusercontent.com/56874442/69976022-a9a3f500-156b-11ea-8715-168bb4b4a97b.png)  
�}6 1/32�T���v�����O

���̂悤�ɃT���v�����O�����傫���Ȃ�ƁC���U�C�N��̃T���v�����O�c�݂���������D
