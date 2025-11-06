clc;
clear;
close all;

% ---------- LOAD IMAGE ----------
img = imread('Radha Krishna.jpg'); % Replace with your image file
if size(img, 3) == 3
    gray = rgb2gray(img); % Convert to grayscale if RGB
else
    gray = img;
end

% ---------- SOBEL EDGE DETECTION ----------
sobel_edges = edge(gray, 'sobel');

% ---------- PREWITT EDGE DETECTION ----------
prewitt_edges = edge(gray, 'prewitt');

% ---------- CANNY EDGE DETECTION ----------
canny_edges = edge(gray, 'canny');

% ---------- DISPLAY RESULTS ----------
figure('Name','Edge Detection Visualizer','NumberTitle','off');

subplot(2,2,1);
imshow(gray);
title('Original Grayscale Image');

subplot(2,2,2);
imshow(sobel_edges);
title('Sobel Edge Detection');
