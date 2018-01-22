clear; % 変数のオールクリア

ORG=imread('Mandrill.bmp'); % 原画像の入力

ORG=rgb2gray(ORG); % カラー画像を白黒濃淡画像へ変換

imagesc(ORG); colormap(gray); colorbar;

pause;

imhist(ORG); % ヒストグラムの表示

![1](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_4-1.png)

図1　グレースケール画像

![2](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_4-2.png)

図2　ヒストグラム
