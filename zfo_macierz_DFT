# Geneorowanie funkcji bazowych dla DFT 
import numpy as np
import matplotlib.pyplot as plt
N = 256     # liczba funkcji bazowych
n = np.arange(N) # numeracja próbek funkcji bazowych
I = np.array( [ np.exp(-2*np.pi/N*k*n*1j) for k in range(N) ] ) # macierz z funkcjami bazowymi 
# zobrazowanie
f = 2
plt.plot(np.arange(N),I[f,:].real,'r',np.arange(N),I[f,:].imag,'k')
f = 254
plt.plot(np.arange(N),I[f,:].real,'g',np.arange(N),I[f,:].imag,'b')
# sygnał analizowany
x=np.sin(2*np.pi*100/256*n)
# obliczenie DFT
P = np.abs( np.dot(I,x) )
# wyświetlanie wyników
k = 100
[ print('{:d}     {:0.3f}'.format(k,P[k])) for k in range(256) ]
k = 0
print('x')
[ print('{:0.3f}'.format(x[k])) for k in range(256) ]
