# bita-rahmani

% خواندن تصویر
image = imread('your_image.jpg');

% ایجاد یک شکل دایره‌ای با قطر ۵۱۲
radius = 256;
center = [256, 256];
theta = linspace(0, 2*pi, 100);
x = radius * cos(theta) + center(1);
y = radius * sin(theta) + center(2);

% نمایش تصویر
figure;
imshow(image);
hold on;

% رسم دایره
plot(x, y, 'r', 'LineWidth', 2);

hold off;
