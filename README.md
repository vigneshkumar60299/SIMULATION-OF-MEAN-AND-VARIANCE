# SIMULATION-OF-MEAN-AND-VARIANCE
## AIM:

To write a program for mean, variance and cross correlation in SCILAB and verify the output.
## EQUIPMENTS Needed

• Computer with i3 Processor • SCI LAB
## Algorithm

   Define the Function: Specify the function you want to simulate. For example, f(x)=sin⁡(x)f(x) = \sin(x)f(x)=sin(x) or any other function.
   Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.
   Evaluate the Function: Compute the function values at each of these sample points.
   Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.
   Display Results: Output the computed mean variance and Cross Correlation PROCEDURE • Refer Algorithms and write code for the experiment. • Open SCILAB in System • Type your code in New Editor • Save the file • Execute the code • If any Error, correct it in code       and execute again • Verify the generated results
   ## program
   ```
   close;
clc;
close;

function X = f(x),
  z = 2 * (3 - x)^3
    X = x * z
endfunction

a = 0;
b = 1;
EX = intg(a, b, f);

function Y = c(y),
  z = 2 * (3 - x)^3
    Y = y * z
endfunction

EY = intg(a, b, c);

disp(EX, "i) Mean of X = ")
disp(EY, "Mean of Y = ")

function X = g(x),
   z = 2 * (3 - x)^3
    X = x^2 * z
endfunction

a = 0;
b = 1;
EX2 = intg(a, b, g);

function Y = h(y),
  z = 2 * (3 - x)^3
    Y = y^2 * z
endfunction

EY2 = intg(a, b, h);

vX2 = EX2 - (EX)^2;
vY2 = EY2 - (EY)^2;

disp(vX2, "ii) Variance of X = ");
disp(vY2, "Variance of Y = ");

x = input("type in the reference sequence = ");
y = input("type in the second sequence = ");

n1 = max(size(y)) - 1;
n2 = max(size(x)) - 1;

r = corr(x, y, n1);
plot2d3('gnn', r);
```
## calculation
![WhatsApp Image 2025-12-04 at 23 08 30_74efed4c](https://github.com/user-attachments/assets/35abcfe2-4400-421e-a083-04e9ba60993e)

![WhatsApp Image 2025-12-04 at 23 08 30_9885cedd](https://github.com/user-attachments/assets/0a7cd322-872c-4560-8eb5-ec323af98729)

![WhatsApp Image 2025-12-04 at 23 09 09_9496fbd2](https://github.com/user-attachments/assets/40eaa647-3870-4bd5-9877-97fd49f1c7ba)

## output 
<img width="1910" height="920" alt="Screenshot 2025-11-19 130126" src="https://github.com/user-attachments/assets/e54b2a11-2fcb-4f0c-b552-b0ad48e3cb05" />

## output waveform

<img width="1900" height="923" alt="Screenshot 2025-11-19 130149" src="https://github.com/user-attachments/assets/5aea323b-4a6f-4fc0-84f9-2990f5a9f828" />

## result
Thus the mean , variance and cross correlation are executed in Scilab and output is verified.




