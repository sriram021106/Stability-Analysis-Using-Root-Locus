# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:
![WhatsApp Image 2025-11-03 at 09 53 47_23ce39f6](https://github.com/user-attachments/assets/1cdd4c07-3c30-4539-9139-fd2b5fa074e9)
![WhatsApp Image 2025-11-03 at 09 55 39_ec169c6d](https://github.com/user-attachments/assets/ec773491-623b-4542-9079-4552631de4c2)
![WhatsApp Image 2025-11-03 at 09 53 48_17b07483](https://github.com/user-attachments/assets/25a0091c-5b4b-4491-b07e-bcd4b9c11bc8)

## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 
~~~
num=[1];
den=[1 15 50 0];
sys=tf(num,den);
rlocus(sys);
[k,poles]=rlocfind(sys)
~~~
## Output:

<img width="1919" height="1048" alt="Screenshot 2025-11-03 094240" src="https://github.com/user-attachments/assets/60a2354b-6432-4414-8684-cb018ffe3af5" />
<img width="1065" height="326" alt="image" src="https://github.com/user-attachments/assets/c1949846-a8c3-4caf-a5f0-8e0a4e08d702" />


## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is  0 < k < 755.9205
