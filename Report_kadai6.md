clear; % 変数のオールクリア

ORG=imread('Lenna.png'); % 原画像の入力

ORG = rgb2gray(ORG);

imagesc(ORG); colormap(gray); colorbar; % 画像の表示

pause; % 一時停止


IMG = ORG>128; % 128による二値化

imagesc(IMG); colormap(gray); colorbar; % 画像の表示

pause;

IMG = dither(ORG); % ディザ法による二値化

imagesc(IMG); colormap(gray); colorbar; % 画像の表示

![1](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_6-1.png?raw=true)

図1　グレースケール画像

![2](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_6-2.png?raw=true)

図2　128による二値化画像

![3](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_6-3.png?raw=true)

図3　ディザ法による二値化画像
