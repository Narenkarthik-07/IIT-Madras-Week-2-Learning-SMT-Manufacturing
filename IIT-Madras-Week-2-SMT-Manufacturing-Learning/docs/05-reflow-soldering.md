# 05 — Reflow Soldering

## Purpose

Reflow soldering heats a PCB assembly containing components placed on solder paste. The paste's solder alloy melts, wets suitable component terminations and PCB pad surfaces, and then solidifies during cooling to create electrical and mechanical connections.

## Typical thermal stages

1. **Preheat:** raises board temperature in a controlled manner and reduces abrupt thermal transitions.
2. **Soak / thermal equalisation (where used):** allows temperatures across the assembly to become more uniform and gives the flux system time to act.
3. **Reflow:** the assembly reaches a temperature sufficient to melt the solder alloy and enable wetting.
4. **Cooling:** the solder solidifies; cooling conditions can influence joint structure and component stress.

The boundaries and control strategy vary with the solder paste, alloy, oven, board mass, and assembly.

## Reflow profile and time above liquidus

A **reflow profile** describes temperature versus time at relevant points on the assembly. Important characteristics may include ramp rate, soak range and duration, peak temperature, time above liquidus (TAL), and cooling rate. Liquidus is the temperature above which the solder alloy is fully liquid.

A suitable profile must balance solder-paste requirements with the thermal limits of components, PCB materials, and other assembly features. The profile should be developed and verified using the paste supplier's guidance, component limits, oven capability, and measurement on a representative assembly.

**No temperature values or profile settings for the IIT Madras equipment are claimed in this repository.** The correct profile cannot be determined from a photograph or machine model alone.

## Air and nitrogen reflow

Reflow can be performed in air or in a nitrogen atmosphere, depending on process requirements and equipment capability. Nitrogen can reduce oxidation in some applications, but whether it is needed depends on solder alloy, flux chemistry, product requirements, cost, and validated process results. It should not be assumed that the pictured line used nitrogen.

## Thermal considerations

- Components have maximum permitted body temperatures and exposure limits.
- Large copper areas and components with different thermal masses heat at different rates.
- Board thickness, copper distribution, panelisation, and component density affect thermal response.
- Thermally sensitive parts may require careful profile validation.
- Measurement locations should represent challenging areas of the assembly.

## Common reflow-related defects

- **Tombstoning:** a small two-terminal component stands up because wetting forces are unbalanced.
- **Solder bridging:** molten solder connects adjacent conductors.
- **Solder balls:** small solder spheres remain around the assembly.
- **Voiding:** gas-related voids remain inside a solder joint; many are not visible to ordinary AOI.
- **Insufficient wetting:** solder does not properly spread over the intended surface.
- **Open or weak joint:** the final connection is incomplete or mechanically inadequate.

Possible causes may originate earlier in printing, placement, component termination condition, pad design, or thermal processing. Defect investigation should consider the full process history.

## Process control

The oven's zones and conveyor conditions are set according to a validated recipe. The recipe must be appropriate to the solder paste, component mix, PCB, and product quality requirements. A machine's displayed settings alone do not prove that the actual board temperature followed the intended profile.

## Training note

Reflow soldering was one of the five SMT stages covered in my Week 2 learning. This document explains the general process; it does not claim a particular profile was measured or run during the training.
