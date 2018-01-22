ORG = imread('Mandrill.bmp'); % 画像の読み込み

ORG = rgb2gray(ORG); % 白黒濃淡画像に変換

imagesc(ORG); colormap(gray); colorbar; % 画像の表示

pause;

IMG = ORG > 128; % 閾値128で二値化

imagesc(IMG); colormap(gray); colorbar; % 画像の表示

pause;

IMG = bwlabeln(IMG);

imagesc(IMG); colormap(jet); colorbar; % 画像の表示

pause;

![1](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_8-2.png?raw=true)

図1　二値化画像

![2](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_8-4.png?raw=true)

図2　ラベル
