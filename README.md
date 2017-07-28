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

Day 1 - Got Arduino To Read a button and a heart rate sensor. Heart Rate sensor seems strange as even when not attached,
it seems to constantly read values around the 500's.

Day 2 - Created a C++ program to read from the Arduino through a serial port, several testing done to figure how to read
values of the arduino properly. Result: since values are between 0-1023, I had to convert that to a string and pad it to
have 4 chars so when I write to serial, the c++ program will constantly receive 6 bytes (4 chars + /r/n). Still some
reading errors, might be due to loop delay in arduino code, reading loop delay in C++ code, or delay in accessing serial.

Day 3 - Spent several hours trying to configure an XBEE, but can't get computer to recognize it.

**Week 7**

Finally got Xbees to communicate. Had to attach TX on Xbee to TX on Ardiuno and same for RX. This allows the arduino to act as a usb to allow configuring the XBee. Then I had to use XTCU to configure the XBees to have the same baud rate, channel, have each other's addresses, and set 1 as router and the other as coordinator.

**Week 8**



**Week 9**

**Week 10**

**Week 11**

