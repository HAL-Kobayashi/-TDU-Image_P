#課題1

#コマンド
ORG=imread('Mandrill.bmp'); % 原画像の入力

imagesc(ORG); axis image; % 画像の表示

IMG = imresize(ORG,0.5); % 画像の縮小

IMG2 = imresize(IMG,2,'box'); % 画像の拡大

imagesc(IMG2); axis image ; % 画像の表示

IMG = imresize(IMG,0.5); % 画像の縮小

IMG2 = imresize(IMG,4,'box') % 画像の拡大

imagesc(IMG2); axis image ; % 画像の表示

IMG = imresize(IMG,0.5); % 画像の縮小

IMG2 = imresize(IMG,8,'box') % 画像の拡大

imagesc(IMG2); axis image ; % 画像の表示

#結果

![1](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_1-1.png?raw=true)

図1　原画像

![2](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_1-2.png?raw=true)

図2　1/2サンプリング画像

![3](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_1-3.png?raw=true)

図3　1/4サンプリング画像

![4](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_1-4.png?raw=true)

図4　1/8サンプリング画像

![5](https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_1-5.png?raw=true)

図5  1/16サンプリング画像
