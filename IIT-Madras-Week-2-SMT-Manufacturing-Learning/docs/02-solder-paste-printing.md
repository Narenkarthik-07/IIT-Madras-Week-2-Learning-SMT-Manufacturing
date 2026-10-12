# 02 — Solder Paste Printing (SPP)

## Purpose

Solder paste printing deposits a controlled quantity of solder paste onto the PCB's surface-mount pads. The deposits provide solder alloy and flux for the later reflow process. Print quality is a major input to downstream placement and solder-joint quality.

## Solder paste: composition and function

Solder paste is generally a mixture of fine solder-alloy particles and flux in a controlled formulation. The metal powder forms the solder joint after reflow. Flux helps remove or manage surface oxides and supports wetting, while the paste's rheology helps it transfer through stencil apertures and retain its shape before placement.

Paste type, alloy, particle size, flux chemistry, storage, handling, and exposure time must follow the supplier's guidance. Different products are not automatically interchangeable.

## PCB pads and stencil apertures

- **PCB pad:** conductive land intended to connect to a component termination.
- **Stencil:** a thin, patterned sheet with apertures corresponding to locations where paste is required.
- **Aperture:** opening through which paste is transferred to a PCB pad.
- **Release:** transfer of paste from the aperture to the pad as the stencil separates from the PCB.

Aperture dimensions and stencil thickness affect the amount and shape of deposited paste. The stencil design must be suitable for the package, pad geometry, paste, and process capability.

## Typical stencil-printer architecture

A stencil printer commonly includes a PCB support and clamping system, stencil frame, alignment system, squeegee assembly, paste handling area, controls, and safety enclosure or guarding. Exact construction and automation differ by model.

The supplied laboratory photograph is labelled as a **GPX-C II** solder paste printer. This identification is based on the visible machine label; no specific configuration or process setting is inferred.

## General printing sequence

1. Load and support the PCB using the approved setup.
2. Align PCB pads with the stencil apertures, using fiducials or the machine's supported alignment method.
3. Apply solder paste to the stencil in accordance with the approved process.
4. Move the squeegee across the stencil so paste fills the apertures.
5. Separate stencil and PCB under controlled conditions so paste transfers to the pads.
6. Inspect the print visually or with SPI before proceeding.
7. Clean the stencil and manage paste according to the work instruction and paste supplier's requirements.

This is a general process description, not a record that I personally executed each operation on the photographed machine.

## Important process parameters

| Parameter | Why it matters |
|---|---|
| Squeegee speed and pressure | Influence aperture filling, paste roll, and transfer |
| Stencil thickness and aperture design | Influence deposit volume and shape |
| Separation speed and distance | Affect paste release and deposit integrity |
| PCB support and clamping | Help prevent board movement or deflection |
| Alignment / registration | Determines whether paste lands on the intended pads |
| Paste condition and handling | Affect print consistency and material behaviour |
| Stencil cleanliness | Residue can obstruct apertures and cause inconsistent deposits |
| Environment and elapsed time | Can affect paste behaviour according to the paste formulation |

Actual settings must be established through validated process instructions, the equipment manual, solder-paste supplier guidance, and suitable process qualification. No IIT Madras machine settings are specified here.

## Common printing defects

- **Insufficient paste:** too little paste transferred to a pad.
- **Excessive paste:** deposit larger or taller than intended.
- **Bridging:** paste joins neighbouring deposits.
- **Misalignment:** deposit is offset relative to the pad.
- **Smearing:** paste is dragged or spread outside the intended deposit.
- **Incomplete transfer / clogging:** paste fails to release consistently from an aperture.

Potential causes overlap. For example, a defect can be influenced by stencil design, paste condition, cleaning, alignment, support, or process settings. Investigate evidence before changing parameters.

## Why print quality matters downstream

Paste deposits influence component seating and the amount of solder available during reflow. Too little paste can contribute to weak or open joints; too much or poorly aligned paste can contribute to bridging or solder balls. SPI provides an opportunity to identify print problems before components are placed, reducing the cost and difficulty of downstream rework.

## Training note

I observed the solder paste printing stage as part of the Week 2 SMT line learning. The photograph in [`../images/solder-paste-printer.jpg`](../images/solder-paste-printer.jpg) shows the GPX-C II printer identified by its visible label.
