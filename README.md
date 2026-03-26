# EXPT 1: Computation-of-DFT-using-direct-method

## AIM
To perform and verify DFT using direct method by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT DIRECT METHOD
    clc;
    clear;
    xn=[1 1 1 1 0 0 2 1];
    n1=0:1:length(xn)-1
    subplot(3,1,1)
    plot2d3(n1,xn);
    xlabel('Time n');
    ylabel('Amplitude xn');
    title('Input sequence');
    j=sqrt(-1);
    N=length(xn);
    Xk=zeros(1,N);
    for k=0:N-1
    for n=0:N-1
        Xk(k+1)=Xk(k+1)+xn(n+1)*exp((-j*2*%pi*k*n)/N);
        
    end
    end
    disp(Xk)

    K1 = 0:1:length(Xk)-1;
    magnitude = abs(Xk);

     subplot(3,1,2);
    plot2d3(K1, magnitude);
    xlabel('frequency(Hz)');
    ylabel('magnitude(gain)');
    title('magnitude spectrum');

    angle = atan(imag(Xk)./real(Xk))

    subplot(3,1,3);
    plot2d3(K1, angle);
    xlabel('frequency(Hz)');
      ylabel('Phase');
    title('Phase spectrum');


### CALCULATIONS:
<br>
<br>
<br>
<br>
<br>
### SAMPLE OUTPUT:
<br>
<br>
<br>
<br>



## RESULT:
Thus,  DFT using direct method for two given sequences were performed and its result was verified.

