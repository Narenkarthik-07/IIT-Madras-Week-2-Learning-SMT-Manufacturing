# 03 — Solder Paste Inspection (SPI)

## Purpose

Solder Paste Inspection (SPI) checks the solder paste deposits after printing and before component placement. It helps determine whether deposits are present, correctly located, and within defined limits for characteristics such as volume, height, and area. SPI results can support print-process monitoring and corrective action.

The supplied laboratory photograph shows a **Koh Young KY8080** system, identified from the visible front label. This repository does not infer its installed options, calibration status, software version, or operating recipe.

## 2D and 3D inspection

| Approach | Typical information | General limitations |
|---|---|---|
| 2D inspection | Image-based deposit presence, apparent area, position, and contrast | Height and volume cannot be directly characterised from a single ordinary 2D image |
| 3D inspection | Surface-height data that can support deposit height and volume estimation, along with area and position | Accuracy depends on the sensing method, calibration, surface properties, setup, and recipe |

Modern SPI systems may use optical techniques such as projected patterns or other height-measurement methods. The exact measurement principle is model-dependent and should be confirmed from the manufacturer's documentation rather than assumed from a photograph.

## Common measurements

- **Volume:** estimated three-dimensional amount of paste in a deposit.
- **Height:** deposit height relative to the measurement reference.
- **Area:** measured footprint of the deposit.
- **Position / offset:** difference between the deposit location and the expected pad location.
- **Presence:** whether a deposit is detected where expected.

Acceptance windows are defined by the product recipe and process requirements. A measured value is not automatically a pass or fail without the applicable limits.

## Typical system elements

An SPI installation may include a camera or optical sensor, illumination or projection hardware, motion system, board transport, image/height processing, inspection software, and a results interface. The specific arrangement depends on the system design.

## Common defects SPI can flag

- Missing or insufficient paste
- Excessive paste volume or height
- Deposit offset or misalignment
- Bridging between adjacent deposits
- Abnormal deposit shape or area
- Inconsistent printing across repeated pads

SPI does not by itself identify the root cause of every defect. Results should be interpreted alongside printer setup, stencil condition, paste handling, board support, and process history.

## How SPI can improve yield

SPI can detect printing deviations before components are placed and the board is heated. Early detection can prevent avoidable downstream defects and provide feedback for process adjustment. The benefit depends on suitable inspection coverage, sensible limits, calibrated equipment, and a controlled response to alarms.

## SPI versus AOI

| Feature | SPI | AOI |
|---|---|---|
| Typical process point | After paste printing, before placement | Commonly after reflow |
| Primary object | Solder paste deposits | Populated PCB and visible assembly features |
| Typical checks | Paste presence, position, area, height, volume | Component presence, orientation, alignment, visible solder-joint features |
| Key limitation | Does not confirm final solder-joint quality | Cannot see every hidden joint or confirm all electrical functions |

## Training note

I learned about the role of SPI in the SMT line and had exposure to the inspection system. The photograph is available at [`../images/solder-paste-inspection-system.jpg`](../images/solder-paste-inspection-system.jpg). No measurement values or inspection results from the training are claimed.
