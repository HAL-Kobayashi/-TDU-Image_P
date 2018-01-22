ORG = imread('Mandrill.bmp'); % 画像の読み込み

ORG = rgb2gray(ORG); % 白黒濃淡画像に変換

imagesc(ORG); colormap(gray); colorbar; % 画像の表示

pause;

imhist(ORG); % 濃度ヒストグラムを生成、表示

pause;

ORG = double(ORG);

mn = min(ORG(:)); % 濃度値の最小値を算出

mx = max(ORG(:)); % 濃度値の最大値を算出

ORG = (ORG-mn)/(mx-mn)*255;

imagesc(ORG); colormap(gray); colorbar; % 画像の表示

pause;

ORG = uint8(ORG); % この行について考察せよ

imhist(ORG); % 濃度ヒストグラムを生成、表示

![1](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_7-1.png?raw=true)

図1　グレースケール画像

![2](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_7-2.png?raw=true)

図2　ヒストグラム

![3](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_7-3.png?raw=true)

図3　濃度値の最大最小値計算後の画像

![4](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_7-4.png?raw=true)

図4　ヒストグラム
