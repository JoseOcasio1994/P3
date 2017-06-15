# Developer's Diary

**Week 2**

Established proposal - create a controller using arduino, which will be a platform
that a user can sit/lie down on and, using 6-axis motion sensors, use their body
to fly in VR.

Planning the design - Used Fritzing to plan visually what the Arduino setup might look like, or
at least how the wiring will be done.
![Arduino Design](https://github.com/JoseOcasio1994/P3/blob/master/Resources/Design.png?raw=true) 

**Week 3**

*Day 1* - Created a project in Unreal and setup the control scheme. Mouse axis controls rotation of Airplane, Arduino will simulate Mouse axis controls. 
Left/Right mouse buttons for firing, Vive controls to be added to replace mouse for shooting.

*Day 2* - Developed a scene for the flight simulation (buildings, targets, and a score manager).

*Day 3* - Started designing the code for the Arduino (Connect to bluetooth, read 
Gyroscope raw data, convert Gyroscope data to Mouse x/y axis, send to PC via bluetooth).

**Week 4**

Did more research on the Vive and Arduino, and looked at the blog of a previous FIEA student who used the arduino.

Vive
- Tracks up to 16 objects
- Has a tracking puck that can be attached to any object that you want to track

Arduino
- Pulse Sensor: detect pulse through finger or earlobe. Another game mechanic?
- Sound Sensor / Mic : detect sound (some brands can detect a range of sound). More game mechanics?
- Joystick library: Code to simulate a Game controller

FIEA-n Blog
- Mapping input values from sensors to desired output range
- Delay loops to properly read sensors
- How to properly use (Read/Write) the sensors
- Create a custom library to hide implementation (so users only see a Update() and Get() call)

**Week 5**

Day 1 - Changed the idea for the game and decided to create a VR Parkour game. Also, decided
to create a File Reader in Unreal so a text file can simulate a heartbeat while I wait
to get parts

Day 2 - Started working on new game design. Completed the File Reader, got a pseudo
heartbeat in, and got basic controls in.

Day 3 - Spent 3 hours trying to get wallrunning in, but failed. Decided to add Timed Doors, 
moving spikes, and booby-trapped mazes. Received parts today.

**Week 6**

**Week 7**

**Week 8**

**Week 9**

**Week 10**

**Week 11**

