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
![原画像]https://github.com/HAL-Kobayashi/TDU-Image_P/blob/master/png_images/PNG_1-1.pngTDU-Image_P/blob/master/img_space/images/1-1.tif?raw=true)  
図1 原画像
