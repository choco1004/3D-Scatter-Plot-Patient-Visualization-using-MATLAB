# 3D-Scatter-Plot-Patient-Visualization-using-MATLAB
3D Biomedical Data Visualization using MATLAB

MATLAB LINK : https://drive.mathworks.com/sharing/4bed6a32-9ec0-4a25-9ff8-3bef3acf135d/%ED%99%98%EC%9E%90%20%EC%83%9D%EC%B2%B4%20%EC%A0%95%EB%B3%B4%203%EC%B0%A8%EC%9B%90%20%EC%82%B0%EC%A0%90%EB%8F%84.m

YOUTUBE LINK: https://www.youtube.com/watch?v=Xkf_z-8gJcQ

clc;
clear;
close all;

% Sample medical data
blood_pressure = [120 130 125 140 135 150 128 132 145 138];
glucose        = [90 110 100 130 125 140 95 105 135 120];
cholesterol    = [180 200 190 220 210 230 185 195 225 205];

% 3D scatter plot
figure;
scatter3(blood_pressure, glucose, cholesterol, 80, cholesterol, 'filled');

grid on;
xlabel('Systolic Blood Pressure');
ylabel('Glucose Level');
zlabel('Cholesterol');
title('3D Scatter Plot of Patient Medical Data');
colorbar;
view(45, 30);
