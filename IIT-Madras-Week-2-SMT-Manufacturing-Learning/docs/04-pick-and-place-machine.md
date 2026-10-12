# 04 — Pick and Place Machine

## Purpose

A pick-and-place machine automatically picks surface-mount components from their supply locations and places them at programmed positions on a PCB. Components are usually placed onto the solder paste deposits before reflow.

The supplied photograph shows a machine bearing the **Yamaha S10** label. The identification is based on the visible marking only; no exact machine capability, installed head configuration, or production speed is asserted.

## Typical machine elements

- **Feeders:** present components from tape, reels, trays, or other supported packaging.
- **Nozzles:** use an appropriate pickup method, commonly vacuum, to hold a component.
- **Placement head:** moves the pickup nozzle between component supply locations and the PCB.
- **Vision cameras:** may inspect component features and PCB references for alignment.
- **PCB transport and clamping:** bring the board into position and hold it during placement.
- **Fiducial recognition:** identifies known board reference marks to correct board-position or rotation offsets.
- **Controller and program:** coordinate component data, feeder assignments, coordinates, orientation, vision checks, and motion.

The exact design differs among machine families.

## General pick, inspect, align, and place sequence

1. The PCB is transported and registered in the machine.
2. The machine identifies board references, such as fiducial marks, where supported by the program.
3. A feeder presents the specified component.
4. A nozzle picks up the component.
5. The machine checks component presence and/or orientation using its supported sensing or vision system.
6. The controller calculates any required correction.
7. The component is placed at the programmed PCB location.
8. The placement program continues through the board's component list.

This is a general sequence; it is not a claim that I ran a placement program during training.

## Component recognition and orientation

The placement program must correctly define the component type, package, position, rotation, and feeder source. Vision systems can use package edges, leads, body features, or other detectable geometry to estimate orientation. Incorrect component data or feeder setup can result in wrong parts, rotated components, pickup errors, or placement offsets.

## Placement accuracy and throughput

Placement accuracy describes how closely a component is positioned relative to its intended location. Throughput describes the amount of work completed over time, often expressed in components per hour or boards per unit time. Real output depends on package mix, board layout, machine configuration, feeder changes, inspection routines, travel distance, and stoppages. Advertised maximum speed should not be treated as the actual line throughput.

## Common placement defects

- Missing component or failed pickup
- Component shifted or rotated from the intended position
- Incorrect component or value loaded in a feeder
- Wrong component orientation or polarity
- Damaged or dropped component
- Placement onto poor, smeared, or misaligned paste

## Why programming and feeder setup matter

The bill of materials (BOM), placement centroid data, component library, board revision, feeder map, and orientation conventions must agree. Independent checks and controlled change management help prevent wrong-part or wrong-orientation assembly. Downstream AOI may detect some visible placement issues, but prevention is preferable to rework.

## Training note

I had exposure to the pick-and-place stage as part of the Week 2 SMT learning. The machine photograph is available at [`../images/pick-and-place-machine.jpg`](../images/pick-and-place-machine.jpg).
