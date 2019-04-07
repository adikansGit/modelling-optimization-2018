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

Mass flow required M = Q/(c_p x dT) = 


Heat demand at Medium Temperature: 9832817 kWh. Over 2245 hours => 4379.873 kW. Maximum heat demand = 6600 kW.
Heat demand at Low Temperature: 18472627 kWh, Over 2245 hours => 8228.341 kW. Maximum heat demand = 12400 kW.

##################################

Low Temperature Heat pump system:

We have a system operating between the evaporator at -0.5 degrees Celsius and the condenser at 55 degrees Celsius. The ideal COP for a heat pump is given as 

COP_ideal = Th/(Th - Tl) = 7.1
Assuming a Carnot efficiency of 0.55, we have an actual COP of 3.9.

The heat pump has 2 heat exchangers and a compressor to be sized, with associated electronics and safety equipment included in the bare module cost factor. 

#Cost of evaporator: Heat load varies from 6000 kW to 7840 kW. U = 484.615 W/m2/C.

#A_evap = 2165.6 m2 to 2830 m2.

#Cost of condenser: Heat load varies from 8060 to 10540 kW. U_cond = 1600 W/m2/C, => U = 414.815 W/m2/C.

Supply temperature = 50 degrees Celsius, => Heat pump condenser temperature = 55 degrees Celsius. Assume the water temperature changes from 50 to 45 degrees in operation. LMTD = 7.213.

#A_cond = 2694 m2 to 3522.6 m2 

CEPCI Index for 2018 = 567.5

<All costs in 1998 USD. It_ref = 389.5 (CEPCI Index)>

Base equipment cost of condenser = 39750 USD to 48986 USD
Base equipment cost of evaporator = 33868 USD to 41159 USD
Material factor for SS tubes and shell instead of carbon steel: 2.86
Adding 80% of the cost for piping (30% for material, 50% for labor) gives us a total bare module factor of 5.15

##Total purchase cost of condenser = 298,265 USD to 367,568 USD
##Total purchase of evaporator = 254,130 USD to 308,838 USD


##Cost of compressor:

#Compressor power varies from 2060 kW to 2700 kW.

We have the compressor cost as a function of flow rate. From some quick back of the envelope calculations, we have the enthalpy change in the compressor (for an ideal case) as 432.9 - 398.5 = 34.4 kJ/kg. This puts the mass flow rate between 60 kg/s and 78.5 kg/s of R134a. This gives us an actual capacity of (60 or 78.5)x0.013738 m3/kg = 0.8243 m3/s to 1.0784 m3/s. In cfm, this is 1746.6 to 2285 cfm. 

Base equipment cost of compressor = 480890 USD to 544850 USD
Adding 174% of the cost for piping and electrical components gives us a bare module factor of 2.74

##Purchase cost of compressor = 1,919,794 USD to 2,175,135 USD


Overall, we have a total cost for the low temperature heat pump varying from 2,472,189 USD to 2,851,541 USD. If we consider the lifetime of the system to be 30 years, and assume a constant interest rate of 8%, the yearly price we pay for the system becomes 170,530 USD to 193,212 USD/year.

If we express this as a function of the compressor power, we have C = 35.44xP + 97522.3125 USD. 

#####################################

#Medium temperature heat pump system:

Condenser temperature = 65 + 5 = 70 degrees Celsius, Ideal COP is 5.6.

For the same Carnot efficiency of 55%, we have an actual COP of 3.07.

Cost of condenser: Heat load varies from 4290 to 5610 kW.

U = 414.815 W/m2/C. Heat pump condenser temperature = 70 degrees Celsius. Water temperature changes from 65 to 60 degrees, giving us an LMTD of 7.213 degrees Celsius.

#A_cond = 1433.8 to 1874.96 m2.

Cost of evaporator: Heat load varies from 2890 kW to 3780 kW.

#A_evap = 1043.1 to 1364.3 m2.


Base equipment cost of condenser = 26107 USD to 31294 USD
Base equipment cost of evaporator = 21779 USD to 25389 USD
Material factor for SS tubes and shell instead of carbon steel: 2.86
Adding 80% of the cost for piping (30% for material, 50% for labor) gives us a total bare module factor of 5.15

##Total purchase cost of condenser = 195,895 USD to 234,815 USD
##Total purchase cost of evaporator = 163,420 USD to 190,492 USD

#Compressor power varies from 1400 kW to 1830 kW.

For the medium temperature system, we assume that the condenser is at 70 degrees Celsius, and for this the enthalpy change in the condenser is equal to 439.8 - 398.5 = 41.3 kJ/kg. This puts the mass flow rate between 34 kg/s and 44.3 kg/s. This gives the actual capacity as (34 or 44.3)x0.009535 m3/kg = 0.3242 m3/s to 0.4224 m3/s. In cfm, this is 686.94 to 895.01 cfm. 

Base equipment cost for the compressor = 357320 USD to 386380 USD
Adding 174% of the cost for piping and electrical components gives us a bare module factor of 2.74

##Purchase cost of the compressor = 1,426,482 USD to 1,542,494 USD

Overall, we have a total cost for the medium temperature heating system varying from 1,785,797 USD to 1,967,801 USD. Expressing this as a function of the compressor power gives us C = 423.265xP + 1193225.84 USD. 

#####################################

