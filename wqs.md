#  problem statement
## ABSTRACT 
- 
INTRODUCTION
MOTIVATION :
NOVELTY of the PROJECT

SCOPE
BASE PAPER
References

approaches 

train a model over known concentrations/ fully concentrated aqueous solutions of top pollutants -- dataset to be experimentally generated, or to be scalped; novel, not been tried

train a model and calibrate it to a specific water source  - wtoh pls 


can gaseous phase uv -vis spectrum be used to get the key features for aqueous phase

tried ftir, have the dataset but organic materials dont show great response to ir spectrum, moreover ftir requires moving parts and high precision

ph turbidity, electro # SeeedStudio Grove EC Sensor Kit (DJS1CBlack ), # SeeedStudio Grove ORP Sensor Kit (501Z), temperature, tds, turbidity


# Working Paper
![[Water-Quality-Sensor-arch.png]]

## Water Quality Assessment parameters
A rapid development in science and technology and a vast usage of industrial processes are generating and releasing more and more pollutants into the environment. The number of pollutants and their concentrations in water are continuously increasing. Therefore, the analysis of chemical pollutants in water has become a serious concern to the professional world and to the authorities in charge of water quality.
^[[WHO-guidelines-drinking-water.pdf]]

 Some of the unique analytical parameter characteristics of the water pollution control industry are biochemical oxygen demand, chemical oxygen demand, acidity, alkalinity, conductivity, hardness, hardness, metal, pH, turbidity tests. Water quality depends on these parameters and their characterization tests.^[[Wastewater Treatment Biological and Chemical Processes by Prof. Mogens Henze, Prof. Poul Harremoës, Dr. Jes la Cour Jansen, Prof. Erik Arvin (auth.) (z-lib.org).pdf]]
 
 Few of them are explained below: 
 ### Alkalinity	
 
 Alkalinity is a measure of the capacity of water to neutralize acids. Alkalinity of water indicates the presence of bicarbonate, carbonate, and hydroxide ions. In waste water treatment, alkalinity is a quality parameter to determine the amenability of waste to the treatment process. Waste water becomes alkaline when receiving alkalinity from the water supply, ground water, domestic use (detergents and soap-based products) and acid rain.
 We can use a pH sensor to determine this parameter.
 
 ### pH
 pH is an important limiting chemical factor for aquatic life. If the water in a stream is too acidic or basic, the H+ or OH– ion activity may disrupt aquatic organisms biochemical re- actions by either harming or killing the stream organisms. pH is expressed in a scale with ranges from 1 to 14. A solution with a pH less than 7 has more H+ activity than OH– , and is considered acidic. A solution with a pH value greater than 7 has more OH– activity than H+ , and is considered basic. The pH scale is logarithmic and making up and down the scale, the values change in factors of ten. An one-point pH change indicates the strength of the acid or base has increased or decreased tenfold.
 
 
 ### Conductivity
 
 Conductivity is a measure of how well water can pass an electrical current. It is an indirect measure of the presence of inorganic dissolved solids. The presence of chloride, nitrate, sulfate, phosphate, sodium, magnesium, calcium, iron and aluminium increases conductivity of water. In addition, organic substances like oil, alcohol, and sugar conduct less electricity which indicates low conductivity of water.
 We can use a Electrical conductivity sensor to estimate this parameter.
 
 ### Hardness
 Hardness is frequently used as an assessment of the quality of water supplies. The hardness of a water is governed by the content of calcium and magnesium salts (temporary hardness), largely combined with bicarbonate and carbonate and with sulfates, chlorides, and other anions of mineral acids (permanent hardness).
 We can use a TDS sensor to estimate this parameter.
 
### Total Solids
Total Solids is a measure of the suspended and dissolved solids in a body of water. Thus, it is related to both conductivity and turbidity. The amount of solids in wastewater is frequently used to describe the strength of the waste. The more solids present in a particular wastewater, the stronger that wastewater will be. Gravimetric is the approved procedure total solids, total dissolved solids, total suspended solids, fixed and volatile solids and Volumetric is the method for measuring settleable solids.
We can use a TSS sensor to approximate this parameter.

 ### Turbidity
 Turbidity is a measure of the cloudiness of water. Cloudiness is caused by suspended solids (mainly soil particles) and plankton (microscopic plants and animals) that are suspended in the water. Moderately low levels of turbidity may indicate a healthy, well- functioning ecosystem, with moderate amounts of plankton present to balance the food chain. However, higher levels of turbidity pose several problems for water systems. Turbidity blocks out the light needed by submerged aquatic vegetation.
 We can use a turbidity sensor to estimate this parameter.
 
 
 ### Chemical Oxygen demand
 COD (Chemical Oxygen demand) is defined as the amount of dissolved oxygen to oxidize and stabilize a sample when organic or inorganic matter of sample solution is responsive by a strong chemical oxidant. The COD value indicates the mass of oxygen consumed per liter of solution and expressed in milligrams per liter (mg/L). The higher the chemical oxygen demand, the higher the amount of pollution in the water sample. However, COD is considered one of the important quality control parameter of an effluent in wastewater treatment facility.
 The complete oxidation of organic compounds under such strong oxidizing conditions produces carbon dioxide (CO2 ) and water (H2O). The COD for any organic compound can be theoretically calculated from writing a balanced equation . 
 Using glucose as an example:
 ![[Pasted image 20210916164531.png]]
 The theoretical COD of glucose can be calculated as:
 ![[Pasted image 20210916164603.png]]
 #### Methods to measure COD
 1. Direct titration using Ferrous Ammonium Sulfate (FAS)
 2.  Potassium Hydrogen Phthalate (KHP) is used as a reference standard for colorimetric analysis
 We will have to get COD values for our samples determined by Biochem Lab at the university.
 ### Biochemcial Oxygen Demand
 BOD is defined as the amount of oxygen required by microorganism to stabilize decomposable organic matter at a particular time and temperature.
 The general form of the equation for decomposition of organic matter during BOD test is
 
 ![[Pasted image 20210916165149.png]]
 
 There is a co-relation between COD and BOD5 and BOD5/COD ratio is known as biodegradability index. Considering domestic wastewaters, this ratio value varies from 0.4 to 0.8 for domestic . If BOD5/COD is ≥ 0.6 then the waste is fairly biodegradable and an effective biological treatment can be possible. If BOD5/COD ratio is between 0.3 and 0.6, then seeding is required to treat it biologically. If BOD5/COD ratio is <0.3 then the probability of biological treatment is less.
 
 #### Methods to measure BOD
 The most conventional method is 5 days BOD determination method. In this standard BOD test, a small sample of the wastewater to be tested is placed along with dilution water in a BOD bottle (300 ml). The Dissolved Oxygen (DO) concentration of the mixture in the bottle is measured. The bottle is incubated for 5 days at 20◦C and the DO concentration is measured again . Oxygen consumed by the organics is determined from the difference and the BOD is calculated as follows:
 ![[Pasted image 20210916165339.png]]
 where,
A1 is the initial concentration DO, mg/L in the dilution water prepared
A2 is concentration DO, mg/L in the diluted sample after 5 days incubation
V1 is the volume of diluted sample
V2 is the volume of the BOD bottle, mL

## UV-VIS Spectroscopy
UV-VIS spectroscopy is the best solution for quantitative determination of organic compounds through absorbance analysis. The UV-VIS spectrometry system is increasingly employed in predicting COD and BOD recently for its significant advantages compared with traditional standard chemical method

When light passes through or is reflected from a sample, the amount of light absorbed is the difference between the incident radiation (Io) and the transmitted radiation (I). The amount of light absorbed is expressed as either transmittance or absorbance. Transmittance usually is given in terms of a fraction of 1 or as a percentage and is defined as follows:
![[Pasted image 20210916165529.png]]
This mathematical formulation was stated by Lambert in 1760 and since then this equation is known by Lambert’s law.
In the later time, the Lambert’s law was combined with an- other law named Beer’s law to produce a relationship between absorbance (A) and transmittance (T). Beer’s law states that the absorption of light is directly proportional to both the concentration of the absorbing medium and the thickness of the medium in the light path
![[Pasted image 20210916165624.png]]
where A is the absorbance,  is the molar absorbtivity (dm3 mol−1 cm−1), c is molar con-
centration (mol dm−3) and b is path length (cm)

# Spectrocopic estimation of COD and BOD

### Proposed Procedure
![[Pasted image 20210916170121.png]]

where, Sλ is sample intensity at wavelength (λ), Dλ is dark intensity at wavelength (λ) and Rλ is reference intensity at wavelength (λ)

### Calibration for waste water COD/BOD determination
Take the influent and effluent samples, measure their COD/BOD values, use them to train ANN or MLR model and calibrate the sensor
### Calibration for water reservoir COD/BOD determination
ANN or MLR Model can be built by training it against the spectral absorbance data and the actual COD/ BOD values.

## what the industry is doing


### UV/Vis spectrometry Solutions by GO Systemelektronik

When light radiates onto a medium - such as water - various effects such as reflection, scattering or absorption occur. Lambert-Beer's law states that the absorption of light at a certain wavelength depends on the concentration of the substance to be measured. UV/Vis spectrometers make use of this effect. Light with wavelengths in the UV and visual range radiates onto the medium, hence the name UV/Vis spectrometry. The substances in the water absorb light of different wavelengths and with different intensity. The remaining light is measured by a detector. The specific absorption per wavelength can then be used to calculate the concentration.
![[Pasted image 20210916111734.png]]
![[Pasted image 20210916111632.png]]
![[Pasted image 20210916111644.png]]
![[Pasted image 20210916111655.png]]

![[Pasted image 20210916111757.png]]

![[Pasted image 20210916111851.png]]

### Realtechwater


## what is ftir, why we proposing uv-vis over ftir

FTIR/ATR Spectroscopy Analysis of COD in Wastewater Based on Combination Optimization of SG Smoothing Modes and PLS Factor

_[Pan, Tao](https://booksc.org/g/Pan,%20Tao "Find all the author's books"), [Ji, Qiang](https://booksc.org/g/Ji,%20Qiang "Find all the author's books"), [Han, Yun](https://booksc.org/g/Han,%20Yun "Find all the author's books"), [Li, Peng Zhao](https://booksc.org/g/Li,%20Peng%20Zhao "Find all the author's books")_

people have made decent specification ftir https://habr.com/en/post/253947/
diy-ftir - check downloads

## what is beer Lambert law, limitations
use the link in the list of links

##

### collection of links
https://guides.lib.utexas.edu/chemistry/spectra -![[Pasted image 20210916112241.png]]
https://spectrabase.com/ - ![[Pasted image 20210916112303.png]]
https://www.researchgate.net/post/UV-Visible-Spectra-Database-can-anyone-help

https://science-softcon.de/spectra/suchen_neu.php?q=aqueous -- aqueous spectrum 
list of spectral databases - https://www.internetchemistry.com/chemistry/spectral%20database.php ![[Pasted image 20210916121335.png]]
nsit database - ![[Pasted image 20210916121533.png]]


### more sensors
EVAL-CFTL-LVDT-ND --- ??
https://robu.in/product/grove-water-atomization-v1-0/ -- atomizer ??
SeeedStudio Grove EC Sensor Kit (DJS1CBlack ) -- elec conductivity


### what does the cwc want

check the cwc-water-quality in downloads


### how do we plan to make the prototype
vu.pdf



