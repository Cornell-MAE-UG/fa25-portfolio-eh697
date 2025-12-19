---
layout: project
title: ENGRD 2210 - Portfolio Assignment
description: Class Assignment
image: /assets/images/kohler-engine.jpg
---

**Collaborators:** _[Susanna Aufrichtig](mailto:sma283@cornell.edu), [Trevor Boshnack](mailto:tjb287@cornell.edu), [Camille Eckert](mailto:cse49@cornell.edu)_

{% raw %}

For this assignment, we will be analyzing and comparing the thermal efficiency of the Rehlko Command PRO CH440 Engine. This is the regulation engine mandated by SAE International for the collegiate Baja SAE Competition. 

Throughout this analysis, most data will be sourced from the manufacturer specification sheet for the CH440 engine and the SAE International Competition Rulebook for the Baja SAE competition.

First, we will model this system as an ideal air-standard Otto cycle.

The efficiency of this ideal system is given by the equation:

$$
\eta = 1 - \left(\frac{1}{r}\right)^{k-1}
$$

where \( r \) is the compression ratio (given by the manufacturer as \( r = 8.3 \)) and \( k \) is the specific heat ratio, typically \( k = 1.4 \) when modeling air as an ideal gas.

Thus we find that:

$$
\eta = 1 - \left(\frac{1}{8.3}\right)^{1.4 - 1} = 0.5711 = 57.11\%.
$$

This is typical for an ideal air-standard Otto cycle.

But how does it compare to the real performance of the engine?

Thermal efficiency of a power cycle in general is expressed as 

$$
\eta = \frac{W_\text{cyc}}{Q_\text{in}}
$$

that is, the work produced by a cycle of work divided by the heat added during this cycle.

To calculate the amount of heat inputted, we analyze the fuel used for the engine and its lower heating value (LHV). For unleaded gasoline, the typical LHV is 12.2 kWh/kg or 43.92 MJ/kg. Baja SAE rules state all competition vehicles must use Pyrotect Part Number SFC100 as a fuel tank. The dimensions of the fuel tank are shown in the drawing (8.00 in ⌀ x 7.94 in). When full, the volume of fuel inside the tank is given by

$$
V = h r^2 = (7.94)(4)^2 = 399.1 \, \text{in}^3 = 0.00654 \, \text{m}^3.
$$

{% endraw %}

<div style="display: flex; justify-content: space-between; align-items: center;">
  <img src="{{ '/assets/images/baja-fuel-tank.png' | relative_url }}" alt="First Image" style="width:48%;">
  <img src="{{ '/assets/images/baja-fuel-tank-drawing.jpg' | relative_url }}" alt="Second Image" style="width:48%;">
</div>

{% raw %}

The typical density for unleaded gasoline is about 0.71 to 0.77 g/mL or 710 to 770 kg/m\(^3\). To be conservative in our calculation of efficiency, we choose the highest density (i.e., a less efficient engine will need more gas to produce the same amount of work). Thus we find that the mass of gas when the gas tank is full is

$$
m = \rho V = (770)(0.00654) = 5.0358 \, \text{kg}.
$$

To calculate the total heat energy that can be obtained from this amount of fuel, we use the previously mentioned LHV value to calculate

$$
Q = m \cdot \text{LHV} = (5.0358) \cdot (43.92) = 221.17 \, \text{MJ}.
$$

Now the trickier part: figuring out how much work we get out of one full tank.

To do this, we will analyze Cornell's vehicle’s motion and fuel consumption during the 4-hour Baja SAE Endurance race. Looking at lap times, track length, and fuel consumption during the last Endurance Race, we find that the vehicle started the race with a full fuel tank and stopped to refuel after.

To find work, we calculate it as

$$
W = F \, dl
$$

and assuming that all force is used to propel the vehicle forward, it can be reduced to

$$
W = F \, l.
$$

To find the length traveled during the consumption of one full fuel tank, we look at the fact that during the most recent endurance race, Cornell’s vehicle stopped to refuel after about 2.25 hours of the endurance race. Looking at the competition’s lap logs, at this time, Cornell had completed 41 laps of the track. Given that one lap of the track at this competition measured about 1.2 miles, we find that the approximate distance traveled by the car on one fuel tank was about 49.275 miles or 79,300.4256 meters. 

To find the average force exerted on the car to move it forward, we perform a static calculation. Taking the coefficient of friction between the wheel and a dirt track to be approximately 

$$
\mu = 0.4,
$$

the free body diagram for one of the wheels looks as below:

{% endraw %}

<div style="text-align: center;">
  <img src="{{ '/assets/images/fbd-baja-wheel.png' | relative_url }}" alt="Centered Image" style="max-width:100%; height:auto;">
</div>

{% raw %}

Multiplying the result of the friction force by four wheels, we find that the total forward force necessary to move the car forward is 889.952 N. 

Going back to the work calculation, we find that the work produced by the engine using up one fuel tank is approximately

$$
W = (889.952)(79,300.4256) = 70.57 \, \text{MJ}.
$$

We can finally return to the efficiency calculation to find that the real-life efficiency of the engine is approximately

$$
\eta_\text{real} = \frac{70.57}{221.17} = 0.319 = 31.9\%.
$$

We find that, as would be expected, the actual efficiency is much lower than the ideal-air standard efficiency. This being said, it is more than obvious that this is not only the product of the real cycle not being ideal air (i.e., not an ideal gas but rather a fuel-air mixture, not isentropic, expansion as a result of combustion rather than heat transfer, etc.) but also due to other broader simplifying assumptions such as assuming only forward motion, assuming constant torque as average torque (when in reality the front and rear wheels produce different amounts of torque at all times and the torque varies between the transmission’s low and high-end ratios), and assuming perfect torque transmission between the wheels and ground (ignoring wheel slip and losses of energy to friction, air resistance, etc.).

{% endraw %}