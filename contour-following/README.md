# Contour Following with a Custom Tool

![16-second loop of the RobotStudio contour-following simulation](../assets/contour-following-preview.gif)

![Close-up of the contour-following station geometry](../assets/contour-following-preview.png)

An individual ABB RobotStudio simulation in which an industrial robot follows programmed contours on three workpieces using a custom tool.

The animation above is a short loop from the simulation. ▶ [Watch the full recorded RobotStudio simulation](../assets/contour-following-simulation.mp4)

## Objective

The objective was to prepare a repeatable robot trajectory along the edges of several objects. The project focused on defining the tool, the work object and the sequence of robot targets required for the simulation.

## Simulation workflow

1. A custom tool and the work object were defined in RobotStudio.
2. Targets were placed along the required contours of the workpieces.
3. The robot program moved the tool through the target sequence to follow each contour.
4. The result was verified in RobotStudio simulation.

## RobotStudio views

### Targets and contour definition

![RobotStudio targets used for contour following](../assets/contour-following-motion-08.jpg)

### Generated robot path

![Robot following the generated contour path](../assets/contour-following-motion-14.jpg)

## 3D station design

Except for the standard ABB robot model, all 3D elements used in this station were designed and created by Piotr Trusiewicz. This includes the workpieces, the custom contour-following tool and the remaining station geometry.

## Files

- [`contour-following.rspag`](station/contour-following.rspag) — ABB RobotStudio Pack & Go archive with the station and RAPID program.
- [`contour-following-preview.gif`](../assets/contour-following-preview.gif) — short animated preview shown directly in this README.
- [`contour-following-simulation.mp4`](../assets/contour-following-simulation.mp4) — recorded execution of the contour-following trajectory in RobotStudio.

## Software

- ABB RobotStudio 2024

## Note

This project was developed and validated as a RobotStudio simulation. It was not deployed in a physical robot cell.
