import numpy as np
import matplotlib.pyplot as plt

# Beginwaarden
dt = 0.25                  #s
t_e = 10                   #s
N = int(t_e/dt)+1
t = np.arange(0,t_e+dt,dt) #s

# fietser 1
x_1 = np.zeros(N)          #m     maakt array van lengte N met alleen maar waarde 0.
v_1 = 5                    #m/s

# fietser 2
x_2 = np.zeros(N)          #m     
v_2 = np.zeros(N)          #m/s     
a_2 = .5                   #m/s^2     

# Uitvoeren van de simulatie
for i in range(0,N-1):
    x_1[i+1] = x_1[i] + v_1*dt
    
    x_2[i+1] = x_2[i] + v_2[i]*dt
    v_2[i+1] = v_2[i] + a_2*dt

# Plotten van de gegevens.    
plt.figure()

plt.xlabel('$t$(s)')
plt.ylabel('$x$(m)')

plt.plot(t,x_1,'r.', markersize=1, label='fietser 1')
plt.plot(t,x_2,'b.', markersize=1, label='fietser 2')

plt.show()



