# 06 — Automated Optical Inspection (AOI)

## Purpose

Automated Optical Inspection (AOI) uses images and software analysis to check visible features of an assembled PCB. It is commonly performed after reflow to help identify assembly defects before boards proceed to further testing or dispatch.

## General inspection principles

An AOI system typically combines cameras, controlled illumination, board positioning or transport, image acquisition, processing algorithms, programmed inspection criteria, and a review interface. Multiple lighting directions, colours, or imaging methods may be used to reveal different features. The exact hardware and algorithms depend on the system.

A programmed inspection compares observed features with expected component locations, package data, reference images, or defined rules. Results are usually classified for review; an alarm does not automatically prove a physical defect.

## Common checks

- Component presence or absence
- Component position, rotation, and skew
- Component polarity or orientation where markings/features are optically distinguishable
- Incorrect or unexpected component appearance
- Visible solder-joint features, such as apparent bridging or abnormal solder shape, where the package and imaging method allow
- Visible damage, lifted leads, or other appearance anomalies within the inspection recipe's capability

## False positives and limitations

AOI can flag acceptable variation as a defect (**false positive**) or miss a defect (**false negative**). Results depend on lighting, camera resolution, board finish, component markings, package geometry, recipe quality, and the limits of optical visibility. Reflective surfaces, occluded joints, and variations in component appearance can complicate inspection.

AOI cannot detect every electrical failure, internal defect, or hidden solder-joint issue. Examples include many hidden joints under bottom-terminated packages, internal voiding, and faults that require electrical or functional testing. X-ray inspection may be appropriate for some hidden joints; electrical tests may be needed to verify function.

## AOI versus SPI

| Aspect | SPI | AOI |
|---|---|---|
| Typical location | After solder paste printing | After component placement and reflow, commonly |
| Inspected material | Paste deposits | Components and visible post-assembly features |
| Typical outputs | Paste height, volume, area, position, presence | Presence, alignment, orientation, visible joint and appearance checks |
| Main value | Detects print issues before placement | Detects visible assembly issues after soldering |
| Important limitation | Does not prove final joint quality | Does not prove all electrical functions or inspect every hidden joint |

## Defect review and corrective action

A flagged board should be reviewed using the system's criteria and an appropriate inspection method. Confirmed defects should be recorded and traced to possible process causes. Repeated false calls may indicate a recipe or lighting issue; repeated genuine defects may indicate a process issue. Changes should be controlled and verified rather than made solely to suppress alarms.

## Training note

AOI was included among the five manufacturing stages covered in my Week 2 learning. No AOI results, defect counts, or machine settings are claimed here.
