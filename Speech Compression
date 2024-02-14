% Speech Compression using LPC
 clear all; 
close all; 
clc;

% Read speech signal 
[x,fs]=audioread('speech.mp'); 
figure(1) 
plot(x) 
xlabel('time(t)') ylabel('amplitude(h(t)') title('original signal')
 % LPC Analysis order 10; 
% LPC order [A, G] lpc(x, order);

% Quantize LPC coefficients A quantized - round(A* 32767); 
% Quantize the speech signal 
xquantized - round(x* 32767); 
figure(2)
plot(x quantized) xlabel('time(t)') ylabel('amplitude(h(t)') title('quantize signal') 
% Save the quantized speech signal and LPC coefficients save('compressed data.mat', 'A quantized', 'G', 'x quantized); 
A-A(1:1); 
% LPC Synthesis
xreconstructed - filter(G, A, x quantized/32767);

% Play original and reconstructed signals

sound(x, fs);

pause(5);

% Wait for the original signal to finish playing

sound(x reconstructed, fs);

plot(x reconstructed) xlabel('time(t)')

figure(3) ylabel('amplitude(h(t)') original bits - numel(x)* 16, 9% 16 bits per sample compressed bits - numel(A_quantized) *16+ numel(G) *16+ numel(x_quantize) 

title('compression signal')

% Calculate Compression Ratio

compression ratio - original bits / compressed bits;

disp(['Compression Ratio: ', num2str(compression ratio)]);
