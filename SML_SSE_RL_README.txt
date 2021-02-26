CREATED BY EVAN C. SNOW ON 01/25/21 FOR SOMATOSENSORY STATE ESTIMATION/REINFORCEMENT LEARNING TASK (Therrien, A. et. al)

SOFTWARE VERSIONS: 
MATLAB 2015a SP1
Dexterit-E3.8

This program is derived from the Weeks et al. 2017 dynamic proprioception task and moved into the vertical (+/- y direction). The movement controller begins all trials by 
passively bringing the participant to a designated starting point recorded in the TP table (from DEX GUI).

In the passive dynamic condition, the robot will move the hand from the starting position. During the movement, a cursor will briefly appear. At the end of the movement, 
participants must report if the cursor was "ahead" or "behind".

In the passive endpoint condition, the robot will move the hand from the starting position to a designated probe somewhere between the start and end points (designated by 
the TP table in DEX GUI). It will then hold the fingertip veridical to the center of the probe and briefly display a cursor. After extinguishing the cursor, the movement 
controller will move the finger tip from the probe to the end target. At the end of the movement, participants must report if the cursor was "ahead" or "behind".

In the active dynamic condition, participants will be held at a start point until a beep sounds, then they begin moving (as instructed). A cursor will appear briefly during 
the movement. The robot will stop the participant's hand at the end point. The participant must then report if the cursor was "ahead" or "behind". A force channel will enforce 
movement direction, and behavioral feedback will be used to maintain movement speed.

In the active endpoint condition, participants will be held at a start point until a beep sounds, then they begin moving (as instructed). A cursor will appear briefly during 
the movement. The robot will stop the participant's hand at the y location of the probe and a cursor will briefly display. After extinguishing the cursor, the participant will 
move the finger tip from the probe to the end target. The participant must then report if the cursor was "ahead" or "behind". A force channel will enforce movement direction, 
and behavioral feedback will be used to maintain movement speed (behavioral feedback for this section is based on both phases individually i.e. start to probe and probe to end).

For all trials, the cursor could be shifted +/- 0, 7, 13, 20, 30, 40 mm. The movement controller constant velocity was set to 0.5 m/s. The cursor was shown veridically 
before movement for 600 ms and somewhere between the start and endpoint (probe location) for 600 ms with logic depending on each task. The recording of the response from the 
patient is recorded using Task Buttons and is evident in the DEX GUI.