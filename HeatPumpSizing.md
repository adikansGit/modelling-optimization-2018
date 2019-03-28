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
A varies from 4457.6 to 5829.2 m2.


