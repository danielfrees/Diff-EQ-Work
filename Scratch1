import numpy as np
from scipy.integrate import odeint
import matplotlib.pyplot as plt
from math import cos
from math import pi

#still trying to figure out what is going wrong with odeint here in this trajectory modeling attempt
def model (c, t):
    return (52+20 *math.cos(2*math.pi/(t-1/3))*c)/100 
                   
#i.c.
c01 = 0.02
c02 = 0.03
c03 = 0.035
c04 = 0.022
                   
                   
#time
t = np.linspace(0, 1000)
                   
#solve
c1 = odeint(model, c01, t)  

                   
# plot results
plt.plot(t,c1)
plt.xlabel('time(years)')
plt.ylabel('pollutant concentration (c)')
plt.show()

#alternate models for different initial conditions, I'll visualize once I get the first function working
c2 = odeint(model, c02, t)                    
c3 = odeint(model, c03, t)                    
c4 = odeint(model, c04, t)
