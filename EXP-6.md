# AIM:
To implement FSK using MATLAB.

# SOFTWARE REQUIRED:
MATLAB

# PROGRAM:
clc;
clear;
close all;

t = 0:0.0001:0.15;

m = square(2*pi*10*t);

c1 = sin(2*pi*60*t);
c2 = sin(2*pi*120*t);

s1 = zeros(size(t));

for i = 1:length(t)
    if m(i) == 1
        s1(i) = c1(i);
    else
        s1(i) = c2(i);
    end
end

figure;

subplot(4,1,1);
plot(t,m);
xlabel('Time (s)');
ylabel('Amplitude');
title('Message Signal');

subplot(4,1,2);
plot(t,c1);
xlabel('Time (s)');
ylabel('Amplitude');
title('Carrier 1 (60 Hz)');

subplot(4,1,3);
plot(t,c2);
xlabel('Time (s)');
ylabel('Amplitude');
title('Carrier 2 (120 Hz)');

subplot(4,1,4);
plot(t,s1);
xlabel('Time (s)');
ylabel('Amplitude');
title('BFSK Modulated Output');

# OUTPUT:
<img width="805" height="513" alt="image" src="https://github.com/user-attachments/assets/7f71e4a1-8e10-47dc-87d1-ca6d083f63b1" />

# RESULT:
Thus, generation of FSK was implemented using MATLAB.



