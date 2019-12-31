# ‰Û‘è‚QƒŒƒ|[ƒg

ORG=imread('Alps.jpg'); % Œ´‰æ‘œ‚Ì“ü—Í  
ORG = rgb2gray(ORG); colormap(gray); colorbar;  
imagesc(ORG); axis image; % ‰æ‘œ‚Ì•\¦

‚É‚æ‚Á‚ÄCŒ´‰æ‘œ‚ğ“Ç‚İ‚İC”’•”Z’W‰æ‘œ‚É•ÏŠ·‚µ‚½Œ‹‰Ê‚ğ}‚P‚É¦‚·D

![Œ´‰æ‘œ](https://user-images.githubusercontent.com/56874442/71593567-0816c000-2b78-11ea-8f45-35df1830aed1.png)  
}1 ”’•”Z’W‰æ‘œ

% 2ŠK’²‰æ‘œ‚Ì¶¬  
IMG = ORG>128;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

![Œ´‰æ‘œ](https://user-images.githubusercontent.com/56874442/71593938-38ab2980-2b79-11ea-9734-7f40c109177c.png)  
}2 2ŠK’²‰æ‘œ

% 4ŠK’²‰æ‘œ‚Ì¶¬  
IMG0 = ORG>64;  
IMG1 = ORG>128;  
IMG2 = ORG>192;  
IMG = IMG0 + IMG1 + IMG2;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

![Œ´‰æ‘œ](https://user-images.githubusercontent.com/56874442/71594178-42815c80-2b7a-11ea-8b38-053e46710944.png)  
}3 4ŠK’²‰æ‘œ

% 8ŠK’²‰æ‘œ‚Ì¶¬  
IMG0 = ORG>32;  
IMG1 = ORG>64;  
IMG2 = ORG>128;  
IMG3 = ORG>160;  
IMG4 = ORG>192;  
IMG5 = ORG>224;  
IMG6 = ORG>256;  
IMG = IMG0 + IMG1 + IMG2 +IMG3 +IMG4 +IMG5 +IMG6;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

![Œ´‰æ‘œ](https://user-images.githubusercontent.com/56874442/71594327-de12cd00-2b7a-11ea-898d-6567848b7707.png)  
}4 8ŠK’²‰æ‘œ
