Notes for Heat pump sizing:


According to this link [1], 57% of EPFL's heating is provided by the heat pump sourced by heat from Lake Geneva. Operating on the assumption that we would like to improve this percentage contribution, we can try to linearize the cost of the heat pump between systems that provide 65 to 85% of the total heating demand. 

https://exploitation-energies.epfl.ch/page-111821-en-html/page-111841-en-html/page-112064-en-html/ 

Heat demand for all of EPFL: 28305444 kWh

Averaged over 2245 hours of heating, this is 12608.2156 kW.

Since the heating demand in the extreme period is likely at least 1.5x higher than a nominal heat load, we take the maximum hourly demand as 19000 kW. Between 65 and 85% of this value is between 12350 kW and 16150 kW.

On the Lake Geneva Side, maximum temperature change is from 6 degrees to 4.5 degrees [2]. => dT = 1.5 degrees.

https://www.swissinfo.ch/eng/sci-tech/renewable-energy_how-to-get-heat-from-the-bottom-of-a-lake/41700430

For the heat pump's evaporator, assuming the dTmin is 5 degrees, the HTF can be at a maximum temperature of -0.5 degrees C. 
LMTD = (dT_hot - dT_cold)/(ln(dT_hot/dT_cold));

LMTD = 5.717 degrees Celsius

Q = U x A x LMTD

1/U = 1/U_1 + 1/U_2

For heat exchange between water and evaporating liquid, these values are taken as 560 W/m2/C and 3600 W/m2/C. => U = 484.615 W/m2/C.

A = Q/(U x LMTD)




Heat demand at Medium Temperature: 9832817 kWh. Over 2245 hours => 4379.873 kW. Maximum heat demand = 6600 kW.
Heat demand at Low Temperature: 18472627 kWh, Over 2245 hours => 8228.341 kW. Maximum heat demand = 12400 kW.

##################################

Low Temperature Heat pump system:

We have a system operating between the evaporator at -0.5 degrees Celsius and the condenser at 55 degrees Celsius. The ideal COP for a heat pump is given as 

COP_ideal = Th/(Th - Tl) = 5.91
Assuming a Carnot efficiency of 0.55, we have an actual COP of 3.25.

The heat pump has 2 heat exchangers and a compressor to be sized, with associated electronics and safety equipment included in the bare module cost factor. 

Cost of evaporator: Heat load varies from 5580 kW to 7295 kW. U = 484.615 W/m2/C.

A_evap = 2014 m2 to 2633 m2.

Cost of condenser: Heat load varies from 8060 to 10540 kW. U_cond = 1600 W/m2/C, => U = 414.815 W/m2/C.

Supply temperature = 50 degrees Celsius, => Heat pump condenser temperature = 55 degrees Celsius. Assume the water temperature changes from 50 to 45 degrees in operation. LMTD = 7.213.

A_cond = 2694 m2 to 3522.6 m2 

Pump power varies from 2480 kW to 3245 kW.




