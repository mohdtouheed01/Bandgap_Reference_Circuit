# CMOS Bandgap Reference Circuit

## Overview

This repository contains the design and simulation of a CMOS Bandgap Reference (BGR) implemented in Cadence Virtuoso.

The design focuses on a temperature-stable reference voltage by combining PTAT (Proportional-To-Absolute-Temperature) and CTAT (Complementary-To-Absolute-Temperature) voltage components.

## Technology

- EDA Tool: Cadence Virtuoso
- Technology Node: GPDK180
- Target Reference Voltage: ~1.2 V

## Design Objective

The objective was to design a CMOS bandgap reference that generates a stable reference voltage while minimizing temperature dependence.

The main parameters studied were:

- Reference voltage
- Temperature coefficient
- Line regulation
- Power consumption
- Supply sensitivity
- PSRR
- Temperature dependence
- Startup behavior

## Circuit Architecture

The bandgap reference combines:

- PTAT voltage generation
- CTAT voltage generation
- Biasing circuitry
- Summing/scaling network

The reference voltage is conceptually obtained as:

\[
V_{REF} = V_{CTAT} + K V_{PTAT}
\]

where \(K\) is selected to achieve temperature compensation.

## Simulation Results

The circuit was analyzed in Cadence Virtuoso using:

- DC analysis
- Temperature sweep
- Supply variation
- Transient analysis
- AC analysis

The simulations were used to study the temperature dependence and stability of the generated reference voltage.

## Layout

The CMOS bandgap reference layout was implemented in Cadence Virtuoso.

Layout screenshots and design files are included in the repository where applicable.

## Verification

The design flow includes:

- DRC
- LVS
- Parasitic extraction, where applicable
- Post-layout simulation, where applicable

## Tools

- Cadence Virtuoso
- Spectre
- GPDK180
