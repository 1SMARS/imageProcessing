I = imread('cameraman.tif');<br>
C = fspecial('average', [3,3]);<br>
d = imfilter(I, C);<br>
<br>
<br>
figure, <br>
subplot(121), imshow(I); title('original');<br>
subplot(122), imshow(d); title('3 x 3 average filter');<br>
<br>
<br>
<br>
<br>
<br>
b = imread('cameraman.tif');<br>
b2 = imdivide(b,64);<br>
bb2 = immultiply(b2,64);<br>
<br>
subplot(121),imshow(b); title('original');<br>
subplot(122),imshow(bb2); title('immultiply');<br>
