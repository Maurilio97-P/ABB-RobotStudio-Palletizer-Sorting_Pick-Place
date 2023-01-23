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

**Note:** the project implements **ISO 10218:2011** to add safety elements for industrial robots

* The main tools used to develop this project are:
  * Smart Components
  * Work Objects
  * RAPID code and Offsets
  * Digital Signals
  * Quickstop 
  * World Zones

## Tutorial:
This simple example was developed to learn the basics of RobotStudio and to make a **step-by-step tutorial** on how to use some of the main tools and to show how to create a new project from scratch. 

[<img src="https://github.com/Maurilio97-P/ABB-RobotStudio-Sorting_Pick-Place/blob/main/Images/thumbnail.PNG" width="50%">](https://youtu.be/y0FjnO8AysQ "Tutorial - Pick&Place con RobotStudio de ABB (Proyecto Final)")

### The tutorial consists of 4 parts:

**Part 1 – Suction Cup with Smart Components**

In this section a .SAT CAD model is imported to generate the gripper in RobotStudio and with Smart Components a sensor is placed on the TCP and the Attach/Detach function is activated with a digital input.

**Part 2 – Conveyor with Smart Components**

In this section, a conveyor is built by applying physical properties to the belt and to the boxes. Sensors are placed at the end of the conveyor and the belt is stopped if a box is detected at the end.

**Part 3 – Pick & Place with Work Objects, Offsets and Digital Signals**

For the Pick & Place, trajectories were made using Work Objects with respect to the conveyor and the 2 pallets near the robot. The creation of boxes and the activation of the suction cup are controlled from the controller using digital input and output signals, finally the Paths are modified to include an offset that allows the boxes to be stacked one on top of the other.

**Part 4 – Security Measures with ISO 10218, QuickStop and World Zones**

Finally, a brief presentation of the ISO 10218:2011 standard is made and the respective CAD models that represent the security elements established in the ISO standard are imported. A QuickStop and Start button is implemented to simulate the scenario in which the light curtain detects a person entering the palletizer and the World Zone function is added to stop the robot if it is inside a special zone defined by the user.

**Unpacking a station (download the .rspag file):**
1. Start RobotStudio and click on the File tab, click Open and then browse to the folder and select the Pack&Go file, the Unpack & Work wizard opens.
2. In the Welcome to the Unpack & Work Wizard page, click Next.
3. In the Select package page, click Browse and then select the Pack & Go file to unpack and the Target folder. Click Next.
4. In the Library handling page select the target library. Two options are available, Load files from local PC or Load files from Pack & Go. Click the option to select the location for loading the required files, and click Next.
5. In the Virtual Controller page, select the RobotWare version and then click Locations to access the RobotWare Add-in and Media pool folders. Optionally, select the check box to automatically restore backup. Click Next.
6. In the Ready to unpack page, review the information and then click Finish.

## Contact Info:
maurilio.pp97@gmail.com

## License
[MIT](https://choosealicense.com/licenses/mit/)
