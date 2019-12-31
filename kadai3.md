# ‰Û‘è‚RƒŒƒ|[ƒg

ORG=imread('Alps.jpg'); % Œ´‰æ‘œ‚Ì“ü—Í  
ORG= rgb2gray(ORG); % ƒJƒ‰[‰æ‘œ‚ğ”’•”Z’W‰æ‘œ‚Ö•ÏŠ·  
imagesc(ORG); colormap(gray); colorbar; % ‰æ‘œ‚Ì•\¦

‚É‚æ‚Á‚ÄCŒ´‰æ‘œ‚ğ“Ç‚İ‚İC”’•”Z’W‰æ‘œ‚É•ÏŠ·‚µ‚½Œ‹‰Ê‚ğ}‚P‚É¦‚·D

![Œ´‰æ‘œ](https://user-images.githubusercontent.com/56874442/71595118-cab53100-2b7d-11ea-892d-b049ca44f94a.png)  
}1 ”’•”Z’W‰æ‘œ

% è‡’l64  
IMG = ORG > 64; % ‹P“x’l‚ª64ˆÈã‚Ì‰æ‘f‚ğ1C‚»‚Ì‘¼‚ğ0‚É•ÏŠ·
imagesc(IMG); colormap(gray); colorbar;

![Œ´‰æ‘œ](https://user-images.githubusercontent.com/56874442/71595363-98580380-2b7e-11ea-8b0e-fbcad5e7bdb1.png)  
}2 è‡’l64

% è‡’l96  
IMG = ORG > 96;  
imagesc(IMG); colormap(gray); colorbar;

![Œ´‰æ‘œ](https://user-images.githubusercontent.com/56874442/71595442-0dc3d400-2b7f-11ea-9569-802b5a74d947.png)  
}3 è‡’l96

% è‡’l128  
IMG = ORG > 128;  
imagesc(IMG); colormap(gray); colorbar;

![Œ´‰æ‘œ](https://user-images.githubusercontent.com/56874442/71595620-bc681480-2b7f-11ea-85d0-9cd7d68f4901.png)  
}4 è‡’l128

% è‡’l192  
IMG = ORG > 192;  
imagesc(IMG); colormap(gray); colorbar;

![Œ´‰æ‘œ](https://user-images.githubusercontent.com/56874442/71595702-110b8f80-2b80-11ea-9bbf-775aacac00b8.png)  
}5 è‡’l192
