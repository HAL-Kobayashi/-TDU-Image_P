ORG = imread('himawari.jpg'); % 画像の読み込み

ORG = rgb2gray(ORG); % 白黒濃淡画像に変換

imagesc(ORG); colormap(gray); colorbar; % 画像の表示

pause;

ORG = imnoise(ORG,'salt & pepper',0.02); % ノイズ添付

imagesc(ORG); colormap(gray); colorbar; % 画像の表示

pause;

IMG = filter2(fspecial('average',3),ORG); % 平滑化フィルタで雑音除去

imagesc(IMG); colormap(gray); colorbar; % 画像の表示

pause;

IMG = medfilt2(ORG,[3 3]); % メディアンフィルタで雑音除去

imagesc(IMG); colormap(gray); colorbar; % 画像の表示

pause;

f=[0,-1,0;-1,5,-1;0,-1,0]; % フィルタの設計

IMG = filter2(f,IMG,'same'); % フィルタの適用

imagesc(IMG); colormap(gray); colorbar; % 画像の表示

pause;

![1](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_9-1.png?raw=true)

図1　グレースケール画像

![2](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_9-2.png?raw=true)

図2　ノイズ添付画像

![3](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_9-3.png?raw=true)

図3　平滑化フィルタ

![4](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_9-4.png?raw=true)

図4　メディアンフィルタ

![5](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_9-5.png?raw=true)

図5　フィルタ適用
