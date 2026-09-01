# AUTOCORRELATION-AND-PSB

EXP NO: 7 SIMULATION OF AUTOCORRELATION AND PSD USING SCILAB

AIM:

Write a program for Autocorrelation and PSD of signals in SCILAB and verify Wiener-Khinchin relation

EQUIPMENTS NEEDED;

· Computer with i3 Processor

· SCI LAB

THEORY:

The Wiener-Khinchin theorem states that the power spectral density of a wide sense stationary random process is the Fourier transform of the corresponding autocorrelation function.

<img width="475" height="86" alt="Screenshot 2026-09-01 222456" src="https://github.com/user-attachments/assets/e0d6ada8-1e5e-4fe4-8c49-808c76436550" />

Algorithm

1. Load or Define the Signal: Input your time-domain signal.

2. Compute Autocorrelation: Calculate the autocorrelation function of the signal.

3. Compute Power Spectral Density (PSD): Estimate the PSD of the signal, either directly using a method like Welch’s periodogram or by using the Fourier transform of the autocorrelation.

4. Plot Results: Visualize the autocorrelation function and PSD.

PROCEDURE

· Refer Algorithms and write code for the experiment.

· Open SCILAB in System

· Type your code in New Editor

· Save the file

· Execute the code

· If any Error, correct it in code and execute again

· Verify the generated waveform using Tabulation and Model Waveform

PROGRAM:

clc

clear all; t=0:0.01:2*pi;

x=sin(2*t); subplot(3,2,1); plot(x); au=xcorr(x,x);

Subplot (3,2,2); plot (au); v=fft(au); subplot(3,2,3);

plot(abs(v)); fw=fft(x); subplot(3,2,4); plot(fw); fw2=(abs(fw)).^2;

subplot(3,2,5); plot(fw2);

OUTPUT WAVEFORM:

<img width="1772" height="866" alt="image" src="https://github.com/user-attachments/assets/37f2ab59-497d-41ed-b1f7-c1f4e35c88e8" />

RESULT:

Thus the Autocorrelation and PSD are executed in Scilab and output is verified.
