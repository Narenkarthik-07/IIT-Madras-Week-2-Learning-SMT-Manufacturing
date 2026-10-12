# 08 — Quality Control and Defects

## Defect reference table

The table below is an educational troubleshooting aid. Causes are possibilities, not definitive diagnoses. A real investigation should use evidence such as inspection images, process records, material condition, component/pad design, and validated measurements.

| Defect | Stage where it may originate | Typical possible causes | Possible detection method | General corrective direction |
|---|---|---|---|---|
| Insufficient solder paste | Printing; stencil design/condition | Aperture blockage, poor transfer, unsuitable print setup, paste condition | SPI; print review | Check stencil cleanliness/design, paste handling, support, alignment, and validated print settings |
| Solder paste bridging | Printing | Excess paste, aperture design, misalignment, smearing | SPI; visual review | Verify stencil/apertures, registration, separation, and paste condition |
| Paste misalignment | Printing / board registration | Incorrect alignment, board movement, fiducial or support issue | SPI | Check registration, clamping/support, board data, and alignment procedure |
| Missing component | Placement / feeder supply | Pickup failure, empty/misloaded feeder, program or recognition issue | AOI; placement records | Verify feeder assignment, pickup/nozzle condition, program data, and component supply |
| Component misalignment | Placement; sometimes paste condition | Incorrect coordinates/rotation, board registration error, unstable paste deposit | AOI; microscope/visual review | Check fiducials, package data, feeder setup, placement program, and paste print |
| Incorrect component polarity | Placement/programming | Incorrect orientation data, component loaded in wrong orientation, unclear marking | AOI where markings are visible; electrical test | Verify BOM, assembly drawing, polarity convention, feeder orientation, and program |
| Tombstoning | Reflow; may be influenced by printing/placement/design | Unequal wetting forces, paste imbalance, pad geometry, thermal imbalance | AOI/visual inspection | Review paste deposits, pad design, placement, component terminations, and thermal profile |
| Solder bridging | Printing / reflow | Excess or offset paste, fine pitch, solder movement during reflow | SPI before reflow; AOI/visual after reflow | Locate origin; review stencil design, print alignment, paste quantity, and reflow conditions |
| Insufficient wetting | Reflow; material/surface condition | Oxidation, unsuitable profile, incompatible materials, contaminated surfaces | AOI if visible; microscopy; joint tests as appropriate | Review material storage, surface condition, paste suitability, and validated thermal profile |
| Solder balls | Printing / reflow | Paste smearing, paste condition, heating/profile issues, surface contamination | AOI/visual inspection | Inspect print and material handling; review profile and board/component conditions |
| Voiding (additional example) | Reflow / pad and package design | Volatile release, paste/flux behaviour, pad design, process conditions | X-ray or suitable specialised inspection | Evaluate requirements, design, materials, and validated process options |

## Quality-control principles

- **Prevent before detecting:** stable printing and correct placement reduce the chance of downstream defects.
- **Use the right inspection stage:** SPI is positioned to assess paste deposits; AOI is positioned to inspect visible assembled features after reflow.
- **Confirm alarms:** automated inspection results need appropriate review, particularly when false calls are possible.
- **Trace upstream:** a defect discovered after reflow may have originated during printing, placement, material handling, or design.
- **Use controlled corrective action:** change one justified factor at a time where practical, document the change, and verify its effect.
- **Respect process documentation:** production settings should follow approved work instructions, equipment guidance, material datasheets, and quality requirements.

## Important caution

A single visible symptom can have several causes. For example, solder bridging may relate to paste volume, stencil aperture design, registration, pad geometry, or reflow behaviour. Do not assume a single root cause without investigation. Corrective actions listed here are general directions, not machine-specific instructions or a substitute for qualified process engineering.
