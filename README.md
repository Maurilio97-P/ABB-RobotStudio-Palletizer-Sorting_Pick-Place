# ABB RobotStudio - Industrial Palletizing Robot - Sorting and Pick&Place Example (IRB 1660ID)
This is a simple example of a sorting and pick&amp;place task simulation for a palletizer using RobotStudio.
<p align="center">
  <img src="https://github.com/Maurilio97-P/ABB-RobotStudio-Sorting_Pick-Place/blob/main/Images/sorting.PNG" width="800" height="450">
</p>

## Requirements:

**Software:**
```bash
ABB RobotStudio 6.08.01
```

**RobotWare:**
```bash
Version 6.08.01.00 (IRB 1660ID)
```

| Software/Package      | Link                                                                                  |
| --------------------- | ------------------------------------------------------------------------------------- |
| ABB RobotStudio       | https://new.abb.com/products/robotics/robotstudio/downloads                           |

## Project Description:
* The palletizer focuses on sorting 2 types of boxes of different height
  * 3 small orange boxes (20x20x10cm)
  * 3 large green boxes (20x20x20cm)
* that the robot must stack on each side
* using a suction cup vacuum gripper

**Note:** the project implements **ISO 10218** to add safety elements for industrial robots

* The main tools used to develop this project are:
  * Smart Components
  * Work Objects
  * RAPID code and Offsets
  * Digital Signals
  * Quickstop 
  * World Zones

## Tutorial:
This simple example was developed to learn the basics of RobotStudio and to make a **step-by-step tutorial** on how to use some of the main tools and to show how to create a new project from scratch. 

[<img src="https://github.com/Maurilio97-P/ABB-RobotStudio-Sorting_Pick-Place/blob/main/Images/sorting.PNG" width="50%">](https://youtu.be/y0FjnO8AysQ "Tutorial - Pick&Place con RobotStudio de ABB (Proyecto Final)")

The tutorial consists of 4 parts:

**Part 1 – Suction Cup with Smart Components**

In this section a CAD model in .SAT format is imported to generate the tool in RobotStudio and with Smart Components place a sensor on the TCP and the Attach/Detach function activated with a digital input.

**Part 2 – Conveyor with Smart Components**

In this section, a conveyor is built by applying physical properties to the belt and to the boxes to be separated. Sensors are placed at the end of the conveyor and the belt is stopped if a box is detected at the end.

**Part 3 – Pick & Place with Work Objects, Offsets and Digital Signals**

For the Pick & Place, trajectories were made using Work Objects with respect to the conveyor and the 2 pallets near the robot. The creation of boxes and the activation of the suction cup are controlled from the controller using digital input and output signals, finally the Paths are modified to include an offset that allows the boxes to be stacked one on top of the other.

**Part 4 – Security Measures with ISO 10218, QuickStop and World Zones**

Finally, a brief presentation of the ISO 10218:2011 standard is made and the respective CAD models that represent the security elements established in the ISO standard are imported. A QuickStop and Start button is implemented to simulate the scenario in which the light curtain detects a person entering the robotic cell and the World Zone function is added to stop the robot if it is inside a special zone defined by the user.
