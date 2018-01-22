clear; % 変数のオールクリア

ORG=imread('himawari.jpg'); % 原画像の入力

ORG= rgb2gray(ORG); % カラー画像を白黒濃淡画像へ変換

imagesc(ORG); colormap(gray); colorbar; % 画像の表示
pause;

IMG = ORG > 42; % 輝度値が42以上の画素を1，その他を0に変換

imagesc(IMG); colormap(gray); colorbar;

pause;

IMG = ORG > 84;　% 輝度値が84以上の画素を1，その他を0に変換

imagesc(IMG); colormap(gray); colorbar;

pause;

IMG = ORG > 126;　% 輝度値が126以上の画素を1，その他を0に変換

imagesc(IMG); colormap(gray); colorbar;

pause;

IMG = ORG > 168;　% 輝度値が168以上の画素を1，その他を0に変換

imagesc(IMG); colormap(gray); colorbar;

![1](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_3-1.png)

図1　グレースケール画像

![2](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_3-2.png)

図2　閾値42の画像

![3](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_3-3.png)

図3　閾値84の画像

![4](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_3-4.png)

図4　閾値126の画像

![5](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_3-5.png)

図5　閾値168の画像
