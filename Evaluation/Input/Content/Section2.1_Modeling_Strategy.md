The general concept of building a PBPK model has previously been described by Kuepfer et al. ([Kuepfer 2016](# 5 References)). Information regarding the relevant anthropometric (height, weight) and physiological parameters (e.g. blood flows, organ volumes, binding protein concentrations, hematocrit, cardiac output) in adults was gathered from the literature and has been previously published ([PK-Sim Ontogeny Database Version 7.3](# References)). The information was incorporated into PK-Sim® and was used as default values for the simulations in adults.

The  applied activity and variability of plasma proteins and active processes that are integrated into PK-Sim® are described in the publicly available PK-Sim® Ontogeny Database Version 7.3 ([Schlender 2016](# 5 References)) or otherwise referenced for the specific process.

The PBPK models were built based on healthy individuals, using the reported mean values for age, weight, height, and genetic background for each study protocol. If no information on these parameters could be found, a healthy male European individual, 30 years of age, with a body weight of 73 kg and a height of 176 cm was used. To model the specific metabolic clearance,  CYP1A2 and CYP2D6 were implemented in accordance with literature, using the PK-Sim expression database RT-PCR profiles ([Meyer 2012](#5 References) )to define their relative expression in the different organs of the body. Glomerular filtration and enterohepatic cycling were enabled, as they are active under physiological conditions.

To distinguish between fluvoxamine metabolism in CYP2D6 extensive metabolizers (EMs) and poor metabolizers (PMs), the CYP2D6 catalytic rate constant (kcat) of PMs was set to zero. This assumption was made because CYP2D6 PMs were characterized by absent CYP2D6 enzymatic activity [Crews 2014](#5 References), which results in a predicted 1.5-fold increase of the fluvoxamine AUC in CYP2D6 PMs compared with CYP2D6 EMs.

Smoking is the strongest known inducer of CYP1A2 and results in higher metabolism of CYP1A2 substrates [Zhou 2009](#5 References). As no detailed information on the frequency, duration, and amount of smoking was available from literature, the induction of CYP1A2 was implemented as a static 1.38-fold increase in enzyme activity. This factor was optimized based on the study of Spigset et al. ,25 resulting in a 39% reduction of the fluvoxamine AUC in smokers.

Unknown parameters (see below) were identified using the Parameter Identification module provided in PK-Sim®. 

The model was then verified by simulating:

- ...

Details about input data (physicochemical, *in vitro* and clinical) can be found in  [Section 2.2](#2.2	Data).

Details about the structural model and its parameters can be found in  [Section 2.3](#2.3 Model Parameters and Assumptions).

