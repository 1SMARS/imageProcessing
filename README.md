I = imread('cameraman.tif');
C = fspecial('average', [3,3]);
d = imfilter(I, C);


figure, 
subplot(121), imshow(I); title('original');
subplot(122), imshow(d); title('3 x 3 average filter');





b = imread('cameraman.tif');
b2 = imdivide(b,64);
bb2 = immultiply(b2,64);

subplot(121),imshow(b); title('original');
subplot(122),imshow(bb2); title('immultiply');
