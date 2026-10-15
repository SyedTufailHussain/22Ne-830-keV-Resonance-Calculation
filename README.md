# 22Ne 830 keV resonance calculation

This is a small notebook I made while studying the paper from the group of Prof. Michael Wiescher at the University of Notre Dame (Shahina et al. 2024) on the 22Ne(alpha,n)25Mg reaction.

In that paper there is a resonance at 830 keV (lab). The paper measured the strength of this resonance for the (alpha,n) channel directly and got 100 +/- 22 micro-eV. An older indirect measurement (Ota et al.) gave 42 +/- 11 micro-eV. I wanted to see how much difference these two values make in the reaction rate inside a star.

For the (alpha,gamma) channel I used 35 +/- 4 micro-eV (Shahina et al. 2022).

## What the notebook does

- Calculates the rate of this single resonance using the narrow resonance formula, for T9 from 0.15 to 1.0
- Plot 1: the full rate curve
- Plot 2: zoom in on T9 = 0.2 to 0.5, where helium burning happens
- Plot 3: the ratio of the (alpha,n) rate to the (alpha,gamma) rate, as a bar chart

## Result

With the direct strength, the neutron rate is 2.38 times bigger than with the indirect one. The ratio (alpha,n)/(alpha,gamma) comes out 2.86 +/- 0.71 for the direct value and 1.20 +/- 0.34 for the indirect value. The paper itself gives 2.85 (71) for this ratio, so my numbers match with the paper.

Only this one resonance is included here, so this is just a check of the effect of the strength, not the full rate.

## Running it

Open the notebook in Jupyter or VS Code and run the cells from top to bottom. It only needs Python 3 and matplotlib.
