# AIM:
To implement ASK, FSK, BPSK using MATLAB.

# SOFTWARE REQUIRED:
MATLAB

 
# PROGRAM:

clc;
t=0:0.0001:0.15;
m = square(2*pi*10*t);
c = sin(2*pi*60*t); y1=(m.*c);
for i = 1:1500 
if(m(i)==1)
y1(i)=c(i);
else y1(i)=0;
end 
end
figure(1) 
subplot(3,1,1); 
plot(m); 
subplot(3,1,2); 
plot(c); 
subplot(3,1,3); 
plot(y1);

# OUTPUT:
<img width="803" height="502" alt="image" src="https://github.com/user-attachments/assets/8566a0a9-c71b-4f2b-8801-c1c6026e26e8" />

# RESULT:
Thus, generation of ASK was implemented using MATLAB.

 

