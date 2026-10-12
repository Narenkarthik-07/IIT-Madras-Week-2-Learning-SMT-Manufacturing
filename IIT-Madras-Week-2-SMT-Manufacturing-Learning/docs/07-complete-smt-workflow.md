# 07 — Complete SMT Workflow

## Representative workflow

![SMT workflow](../diagrams/smt-process-flowchart.png)

1. PCB preparation
2. Solder paste printing
3. Solder Paste Inspection (SPI)
4. Component pick and placement
5. Reflow soldering
6. Automated Optical Inspection (AOI)
7. Defect review and corrective action
8. Further testing, if required

This is a representative workflow, not a universal factory layout. Some lines include additional inspection, cleaning, traceability, routing, X-ray inspection, depanelisation, in-circuit testing, or functional testing. Some production flows also assemble the opposite side of a PCB in a separate sequence.

## Stage-by-stage purpose and dependency

| Stage | Purpose | Influence on the next stage |
|---|---|---|
| PCB preparation | Confirm correct board, revision, condition, and support/handling setup | Incorrect board revision or damage can invalidate later work |
| Solder paste printing | Deposit paste on intended pads | Paste quantity and position affect component seating and solder availability |
| SPI | Check paste deposits against programmed criteria | Print defects can be corrected before placement and reflow |
| Pick and place | Put correct components at intended positions and orientations | Wrong, missing, or shifted components can create assembly defects |
| Reflow | Melt and solidify solder to form joints | Thermal profile and wetting affect joint integrity |
| AOI | Inspect visible post-reflow assembly features | Identifies issues for review before later process steps |
| Defect review | Confirm calls, determine probable causes, and decide disposition | Feedback can improve process control and prevent recurrence |
| Further testing | Verify electrical or functional requirements as applicable | Detects faults that optical inspection cannot establish |

## Why the workflow is connected

A final solder-joint defect may be related to paste deposition, component placement, surface condition, or the thermal profile. For that reason, troubleshooting should consider upstream records and process conditions instead of assuming that the stage where a defect is found is necessarily where it originated.

## Feedback and traceability

A controlled manufacturing process may record board identifiers, program revisions, inspection results, component/feeder data, profile measurements, and repair outcomes. Traceability makes it easier to compare recurring defects and verify whether a corrective action works. The specific traceability system used in the photographed laboratory was not documented in this learning record.

## Learning reflection

My Week 2 learning focused on understanding the roles of SPP, SPI, pick and place, reflow, and AOI as connected stages in an SMT fabrication line. The main insight is that quality depends on the interaction of these stages, not on any single machine alone.
