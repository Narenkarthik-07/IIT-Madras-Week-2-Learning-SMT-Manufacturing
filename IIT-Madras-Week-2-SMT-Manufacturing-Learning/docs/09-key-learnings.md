# 09 — Key Learnings from Week 2

## Learning summary

Week 2 of the Advanced Electronics Manufacturing Training Program at the Central Electronics Centre, IIT Madras, provided hands-on exposure to an SMT fabrication line. The learning covered five connected stages: solder paste printing, solder paste inspection, pick-and-place placement, reflow soldering, and automated optical inspection.

## Key technical learnings

### 1. SMT is a sequence of interdependent operations

Each stage prepares the PCB for the next one. A print defect can affect component placement and solder formation, while incorrect component placement can remain a problem even when the reflow process is suitable.

### 2. Inspection supports process control

SPI can identify paste-deposit deviations before placement. AOI can inspect visible assembly features after reflow. These systems serve different purposes and neither replaces every other form of inspection or electrical testing.

### 3. Automation depends on correct setup and data

Stencil design, board alignment, component data, feeder assignments, placement programs, and inspection recipes all influence process consistency. Automation does not remove the need for correct engineering inputs and review.

### 4. Reflow is a controlled thermal process

A suitable thermal profile must match the solder paste, PCB, and component limits. It should be established and verified using technical documentation and representative measurements—not guessed from the oven's appearance.

### 5. Defect prevention requires a process-wide view

The point where a defect is detected may not be the point where it originated. Effective investigation considers the whole assembly flow and uses evidence before selecting corrective action.

## What this record does and does not claim

**Reported learning/exposure:** hands-on exposure to the SMT fabrication line and learning about the five stages listed above.

**General educational content:** the process explanations, parameter considerations, defect examples, and glossary in this repository.

**Not claimed:** independent operation of every machine, specific experiments, measured results, production quantities, exact machine settings, defect rates, or qualifications not provided in the training information.

## Next steps for continued learning

- Read equipment and solder-paste supplier documentation relevant to the process.
- Study PCB land patterns, stencil design, and design-for-manufacturing considerations.
- Learn how process windows are established and verified through controlled trials.
- Explore inspection examples and understand how false positives and false negatives are managed.
- Study the applicable quality requirements for the intended product class.
