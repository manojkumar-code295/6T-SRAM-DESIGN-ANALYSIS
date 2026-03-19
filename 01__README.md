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
## 🔍 Observations & Insights

### Butterfly Curve
The butterfly curve is used to analyze SRAM stability. It is formed due to cross-coupled inverters. It helps measure SNM, which indicates noise tolerance.

### Read Operation
During read, slight disturbance occurs in the stored data due to bitline interaction.

### Write Operation
Write operation flips the stored data when sufficient voltage is applied.

### Corner Analysis
Performance varies with process, voltage, and temperature conditions.

### Transient Response
Shows how the SRAM responds over time during switching.

## 💡 Key Learnings
- Understood SNM and stability of SRAM
- Learned read disturb and write ability
- Analyzed impact of PVT variations

## 👨‍💻 Author
Manoj Kumar R

## RESULTS
## 📊 Results
![Butterfly Curve](04_results/butterfly_curve.png.img)
![Corner Analysis](04_results/corner_analysis.png.img)

