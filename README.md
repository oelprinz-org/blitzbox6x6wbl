# blitzbox6x6wbl - first draft version<br/>
blitzbox6x6wbl - low-cost and mini-sized 6x6 ECU for rusefi (and probably speeduino) firmware (45 x 50 mm) 
<br/>

ultra-low-cost and mini-sized ECU for rusefi firmware (Rev0.0.1 45 x 50 mm)<br/>
Integrated Wideband Lambda Controller with Bosch LSU 4.9 sonde<br/>
4-Layer highly integrated design - hand soldering possible but only recommended to people with really experienced soldering skills.  Hardware is optimized for assembly by professional assembly manufacturer<br/>
supports 6 cylinder full sequential<br/>

6 high impedance injectors (Injector 5 and 6 shared with idle valve output)<br/>
6 active ignition coils<br/>
1 crankshaft sensor with MAX9924 VR-conditioner<br/>
1 hall input for camshaft sensor<br/>
6 analog inputs: CLT, IAT, TPS, Spare analog input, MAP or Baro onboard MPXH6400A<br/>
1 digital input for disco swaggering (aka. launch control)<br/>

1 fuel pump out<br/>
2 idle valve out<br/>
1 tacho out (5/12V)<br/>
1 fan out<br/>

USB-C programming interface onboard<br/>
Wireless Tunerstudio connection WIFI/BT via ESP32-C5<br/>

21.01.2026: Betaversion 0.0.1 first draft - More infos coming soon....<br/>

[Link to the rusefi project](https://www.rusefi.com "rusefi homepage")<br/>
<br/>
Quick link to Rev0.0.1 schematic: https://github.com/oelprinz-org/blitzbox6x6wbl/blob/master/hardware/Rev0.0.1/schematics_blitzbox6x6wbl.pdf <br/>



### Bosch CJ125 (LQFP32 package) part numbers

|Bosch part number|
|:----------------|
|30615|
|40103|
|30522|

### Suitable Bosch lambda probes

Basically, the Bosch probes whose numbers start with **0 258 017** will fit, also Bosch **0 281 004**.  
Bosch numbers beginning with **0 258 007** are *LSU 4.2* probes and will not fit.

|Bosch number  |Length overall|Comment|
|--------------|--------------|-------|
|0 258 017 012 |1060mm||
|0 258 017 025 |1000mm|Bosch motorsport part|
|0 281 004 028 |540mm|common probe for diesel engines|
|0 258 017 029 |620mm|grey, used by BMW after 09/2006 (1178 7539124)|
|0 258 017 038 |340mm|grey, used by BMW (11787537984)|
|0 258 017 092 |950mm|black, used by BMW (1178 7540167)|
|0 258 017 126 |680mm|black, used by BMW after 09/2006 (1178 7561410)|
|0 281 004 150 |1215mm||
|0 281 004 184 |1000mm||
|...|||

### LSU4.9 probe pinout

|Pin#|Color|Description|Symbol|
|----|-----|--------|-----------|
|1|red|Pump current APE|IP|
|2|yellow|Virtual ground IPN|VM|
|3|white|Heater voltage H-|Uh-|
|4|grey|Heater voltaget H+|Uh+|
|5|green|Trim Resistor RT|IA|
|6|black|Nernst voltage UN|RE|


<p align="center">
  <br/>
  <img src="hardware/Rev0.0.1/2022-09-22-Board-Blitzbox-V0.1.3_top.png" width="710" alt="Board-Blitzbox-V0.1.3_top"><br/>
  <img src="hardware/Rev0.0.1/2022-09-22-Board-Blitzbox-V0.1.3_bottom.png" width="710" alt="Board-Blitzbox-V0.1.3_bottom"><br/>
  <img src="hardware/Rev0.0.1/2023-05-15-Board-Blitzbox-V0.1.9.png" width="710" alt="Board-Blitzbox-V0.1.8"><br/>
  <img src="hardware/Rev0.0.1/top.png" width="350" title="top">
  <img src="hardware/Rev0.0.1/bottom.png" width="350" alt="bottom"><br/>
  <img src="hardware/Rev0.0.1/internal_plane1.png" width="350" title="Internal Plane 1">
  <img src="hardware/Rev0.0.1/internal_plane2.png" width="350" title="Internal Plane 2">
  <img src="hardware/Rev0.0.1/top_layer.png" width="350" title="top_layer">
  <img src="hardware/Rev0.0.1/bottom_layer.png" width="350" alt="bottom_layer">
  <img src="hardware/Rev0.0.1/assembly_solderside_V0.1.9.png" width="710" alt="assembly_solderside"><br/>
  <img src="hardware/Rev0.0.1/assembly_connectorside_V0.1.9.png" width="710" alt="assembly_connectorside"><br/>
</p>
<br/>
<p align="center">
  <br/>
</p>
