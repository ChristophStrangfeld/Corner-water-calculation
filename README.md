# Corner-water-calculation
This is the corresponding code for the publication "Quantification of physisorbed and corner water in partially saturated pore networks based on polygonal pore geometries".

This repository contains MATLAB scripts for the processing of pore saturations and sorption isotherms for different pore geometries and materials. Furthermore, it contains experimental data, including pore volume distributions (PVD) and measured sorption isotherms.

The Matlab-file main_program.m reads in the measurement data and physical constants for subsequent calculations. This includes experimental data of 36 materials: earth, sandstone, cement-based screed and calcium-sulphate-based screed. 
Calculations include the prediction of the pore saturation for different geometries such as slit-shaped, cylindrical, spherical, equilateral triangular, isosceles triangular, square, and hexagonal pores. 

The main objective is to calculation physisorbed and condensed water in partially saturated pore and materials throughout the hygroscopic range.

📌 Overview

The MATLAB script main_program.m performs the following tasks:

Reads the measured PVD and sorption isotherms.

Read physical constants for subsequent calculations.

Computes the saturation of individual pores with different geometries.

Separates adsorbed and condensed at partial saturation.

Computes the sorption isotherm for 36 investigated materials and quantifies the ratio of condensed water. 

🧪 Experimental Setup

Investigated materials:

3DF_50

Bozanov

Brenna

Brenna_2020

Gravenhorster

Ilsfelder

Knauf_FE_25_A_Tempo

Knauf_FE_50_Largo

Knauf_FE_80_Allergo

Kylltaler

Kylltaler_2020

LSW_50

Lichtenberger

Lichtentaeler

M2_50

M3_50

MW_50

Maulbronner

NF_50

Neckartaeler

Neuheilenbacher

Obersulzbacher

Pfaffenhofer

Remlinger

Roettbacher

Sakret_Beton_Estrich

Sander

Santa_Fiora

Schleeriether

Schoenbrunner

Skala

Udelfanger

Weber_floor_4060

Weber_floor_4065

Weber_floor_4341

Weber_floor_4490

The PVD were determined with mercury intrusion porosimetry and gas adsorption according to ISO 15901-1:2016 and ISO 15901-2:200. The sorption isotherms of screed samples were measured in climate chambers, for sandstones in desiccators, and earth in dynamic vapour adsorption devices. Measurements were taken always at equilibrium state.

📁 Data Structure

The measurement data must follow the directory structure below:

For each material, a file exists for the pore volume distribution "pore_volume_distribution_#material_name#".

For 28 materials, measured sorption isotherms are available. The corresponding files are named "sorption_isotherm_#material_name##

⚙️ Data Processing

Individual pore saturation is calculated for cylindrical pores based on Hillerborg sorption theory.

Individual pore saturation is calculated for slit-shaped pores based on BET sorption theory.

Individual pore saturation is calculated for equilateral triangular pores: I- pure adsorption based on BET sorption theory, II- pure condensed water based on Kelvin equation, III- combination of both.

Individual pore saturation is calculated for isosceles triangular pores: I- pure adsorption based on BET sorption theory, II- pure condensed water based on Kelvin equation, III- combination of both.

Individual pore saturation is calculated for square pores: I- pure adsorption based on BET sorption theory, II- pure condensed water based on Kelvin equation, III- combination of both.

Individual pore saturation is calculated for hexagonal pores: I- pure adsorption based on BET sorption theory, II- pure condensed water based on Kelvin equation, III- combination of both.

For 36 materials, the sorption isotherm is calculated for cylindrical pores based on Hillerborg sorption theory.

For 36 materials, the sorption isotherm is calculated for slit-shaped pores based on BET sorption theory.

For 36 materials, the sorption isotherm is calculated for equilateral triangular pores: I- pure adsorption based on BET sorption theory, II- pure condensed water based on Kelvin equation, III- combination of both.

For 36 materials, the sorption isotherm is calculated for isosceles triangular pores: I- pure adsorption based on BET sorption theory, II- pure condensed water based on Kelvin equation, III- combination of both.

For 36 materials, the sorption isotherm is calculated for square pores: I- pure adsorption based on BET sorption theory, II- pure condensed water based on Kelvin equation, III- combination of both.

For 36 materials, the sorption isotherm is calculated for hexagonal pores: I- pure adsorption based on BET sorption theory, II- pure condensed water based on Kelvin equation, III- combination of both.

📦 Key Output Variables

Saturation of individual pores in respect to humidity, geometry, adsorption and/or condensation.

Material moisture in respect to humidity, geometry, adsorption and/or condensation.

Contribution of condensation of the material moisture.

📈 Additional Data Extraction

Validation of the snap-off criterion when the corresponding relative humidity is approaching the water-vapour partial pressure at saturation. 

🛠 Requirements

MATLAB (recommended: R2024b or newer)

👤 Author / Context

Christoph Strangfeld
