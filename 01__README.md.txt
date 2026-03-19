#6T SRAM Design and Analysis

##overview
This project demonstrates the design and analysis of a 6T SRAM cell

##Features
-Butterfly curve(SNM ANALYSIS)
-READ and WRITE operations
-Corner analysis
-Transient response

##Folder structure
-Schematics/
-simulations/
-results/ 

##observations and insights
6T SRAM stores data using a bistable latch formed by cross-coupled inverters (basically 2 PMOS- pullup, 2 NMOS- pulldown, 2NMOS- Access transistors)
It operates in two modes: Hold on and Read mode 
-HOLD MODE 
 	When WL=0, access transistors are turned off, and data remains there only here. Transistor stability is higher, no external disturbance, and the SNM ratio is maximum.
-READ MODE
	When WL = 1, Access nodes connect QB to BLB(HIGH), there is an external disturbance, SNM is low, and data flipping is possible 
-VTC/VDC Graph
It is a voltage relationship between the input and output voltage of an inverter inside the SRAM cell, where the voltage varies from 0 to VDD
A steeper curve means higher gain and better noise immunity 
As the input is low, the output is high. As the input rises, the output threshold gradually decreases
-Butterfly curve
This curve is used to check the stability of the SRAM.
It is made by plotting two inverter characteristics.
By this curve, one inverter uses the logic 1, and the other uses the logic 0, and when both overlap, this creates a 
butterfly curve. Why do we need this? Because the noise is always present, and voltage fluctuations happen.
SNM creates the strength of stability.
-Corner Analysis
It is performed in SRAM for  robustness under real-world variation
In particular, semiconductor fabrication, parameters such as transistor speed, threshold voltage, temperature and supply voltage can vary
-pre-corner analysis 
It was performed under typical conditions to verify the 6T SRAM

## RESULTS
Successfully designed and analysed a 6T SRAM cell, verifying correct functionality in hold, read, and write modes.
Evaluated stability using VTC and butterfly curves, confirming reliable operation through sufficient static noise margin (SNM).
Validated robustness of the design through pre-corner and corner analysis, ensuring proper performance under different conditions.     
