clear; % 変数のオールクリア

ORG=imread('himawari.jpg'); % 原画像の入力

ORG = rgb2gray(ORG); colormap(gray); colorbar;

imagesc(ORG); axis image; % 画像の表示

pause; % 一時停止

% ２階調画像の生成

IMG = ORG>128; 

imagesc(IMG); colormap(gray); colorbar;  axis image;

pause;

% ４階調画像の生成

IMG0 = ORG>64;

IMG1 = ORG>128;

IMG2 = ORG>192;

IMG = IMG0 + IMG1 + IMG2; %384

imagesc(IMG); colormap(gray); colorbar;  axis image;

%　８階調画像の生成

IMG0 = ORG>32;

IMG1 = ORG>64;

IMG2 = ORG>96;

IMG3 = ORG>128;

IMG = IMG0 + IMG1 + IMG2 + IMG3; %418

imagesc(IMG); colormap(gray); colorbar;  axis image;




![2](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_2-1.png)
図1　グレースケール画像


![3](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_2-2.png)
図2　2階調画像の生成


![4](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_2-3.png)
図3　4階調画像の生成
