# Sensor-Based Pick and Place

![RobotStudio sensor-based pick-and-place station preview](../assets/sensor-pick-place-preview.png)

An individual ABB RobotStudio simulation of bidirectional block transfer between two tables.

## Logic

1. A virtual line sensor checks whether the block is present on the first table.
2. If detected, the robot approaches the block with an open custom gripper.
3. The jaws close and the simulation attaches the block to the gripper.
4. The robot transfers the block to the opposite table, releases it and detaches it from the gripper.
5. If the first table is empty, the control logic checks the other table and performs the same sequence in the reverse direction.

## Files

- [`sensor-based-pick-and-place.rsstn`](station/sensor-based-pick-and-place.rsstn) — RobotStudio station.
- [`robot-gripper-jaws.ipt`](cad/robot-gripper-jaws.ipt) — Autodesk Inventor source model.

The project was developed and validated as a RobotStudio simulation. It was not deployed in a physical robot cell.

## 3D station design

Except for the ABB robot model, every 3D element in this station was designed and created by Piotr Trusiewicz. This includes both tables, the transferred workpiece, the custom gripper and its jaws, and the remaining station geometry.

![Custom gripper jaws designed for the station](../assets/robot-gripper-jaws-cad.png)
