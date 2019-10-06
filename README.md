# ACIM5010-PLC-Project
Allen-Bradley 1769-L32E CompactLogix Bin Sorting Project for BCIT

Programmed in Ladder Logic

May 2019 for ACIM 5010

General Description:
Two separate bins will be filled each with a pre-determined number of items.  The conveyer that is loading the bins will shut down when the sweep arm is making the transition from filling one bin to another.This system consists of:            
-  A single emergency stop
-  A single stop push button and a single start push button
-  Three limit switches (normally closed)
-  A green lamp will flash when conveyer is in motion and photo eye actuated.              
-  An amber lamp will flash when loading arm is in motion.
-  A red lamp will indicate that a bin is loading
-  A forward/reversing starter.                 
-  A single starter

System Design
The system will be initiated by pressing the start button, the process will start to fill bin one. If the start button is pressed and neither bin limit is actuated the gate motor will run in the direction allowing for Bin 1 to be filled.  Once the limit is actuated the process will start. When the conveyer is filling the bins the green light will be on and flash when the photo-eye(limit 3) is actuated. When the gate motor is running the amber light will flash in increments of 1 second. When the bin limit is made the conveyor will start. The photo-eye will count five boxes then switch to fill the other bin. When the wiper is in motion the conveyor will not run. A stop button will stop the process such that the current count will end then the system will stop regardless of the bin being filled. If the stop button is pressed while the wiper is in motion then the system will just stop.
