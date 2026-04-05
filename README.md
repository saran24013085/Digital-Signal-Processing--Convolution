# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 

clc; % clear screen
%clear all; % clear screen
close all; % close all figure windows

% input sequence
% X[n]={2,−1,4−2.3,5,9,−3} h[n]={3,−4,1,1,2.7,3.5,2}

a = input("enter the starting x(n)");
x = input("enter the x(n) sequence");
n = a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

%impulse sequence

b= input('enter the starting h(n)');
y = input('enter the h(n) sequence');
m = b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

%linear convolution

z = conv2(x,y);
n1 = a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');

## OUTPUT:
<img width="1920" height="1200" alt="Screenshot (468)" src="https://github.com/user-attachments/assets/d02aa28f-6b32-42fa-aa83-26c2a7ad3a1d" />
<img width="1920" height="1200" alt="Screenshot (469)" src="https://github.com/user-attachments/assets/eca1cf06-01c5-43f8-bb49-823eec0c06fb" />
<img width="1920" height="1200" alt="Screenshot (470)" src="https://github.com/user-attachments/assets/4d4fee17-7ab0-4956-98f8-bb32a5c9f1af" />


## RESULT:
![exp 1 result](https://github.com/user-attachments/assets/3d7b52c8-263d-4f05-8b92-3c8e1793666b)




