# COB1-Repository
Repository for COB1 robot for Children of the Corn.

- Se and PlotSmoothPath - Se uses the forked algorithm from KHEngineering. It basically allows you to set waypoints for the robot to drive through. See https://github.com/Team6945/SmoothPathPlanner
  - S1 has no syntax errors. Logically should work (tested in another program)
  - S2 - added TenFeet command to calibrate max Velocity of the robot for AutoPath
  - S3 added possible paths to use and appropriate selector. Once maxV is calculated, modify times for max efficiency. -4/2, updated 4/8 --NOT WORKING YET
    - some angles in the auto Twice might need negatives
  - S3pidturn - S3 edited to use pid turning for auto Twice commands (in case the robot turns when taking from the pyramid). -4/2
    - needs to be tuned; if not working, scrap it 
    
   -SFINAL: working smooth path program - multipliers set for COB1

- P9 - first week comp - 3/12

- C1 must be edited; should work, so autonomous can be selected based on game data - 3/12
- C2 adds (maybe) correct measurements to C1 for AP2RSwitch & AP2LSwitch - 3/12
- C3 has updated speed values - 3/13
- *C4 does not exist because surperstition since C4 is an explosive (-Adam - 3/13)*
- C5 Ramp-down on the teleoperated, UNTESTED. Also, AutoInit (should) select correct command group based on selections from the smartdashboard and randomized game data. - 3/13
- C6 Removed ramp-down on teleop, doesn't work well. Added overdrive button - 3/14
- C8 WORKS - code used in finals of Bridgewater-Raritan event - 3/16
- C11 adds switch capabilities to driver station 1 and 3 in auto, providing that the friendly switch is on that side

- T1 is a copy of C11, adds timer to smartdashboard
- T2 replaces the count down timer with a count up for showcases and races. Also inverts the right block sucker motor due to new wiring
