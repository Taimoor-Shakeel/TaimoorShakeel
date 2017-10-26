# Line Following Lego Robot

## Description of Project
Line Following Lego Robot using PID Controller

Line following is the the most useful applications for robots, because it allows the robot to move from one point to another to do several tasks without any assistance.

## Description of the Work Process

Problems I faced 
- How to connect the lego components and what would be the size of it.
- Fist to decide which software is appropriate to work with lego robot so in order to have good results and in time.So I do some tests  
  with matlab and EV3 softwares.
- Don't know how to load the code and make a setup connection between lego robot and software via bluetooth and WIFI.
- How to make the code run on hardware directly. robot and software via bluetooth connection and WIFI.
- How to use different sensors and calibrate them.
- How to use PID controller and tune it in software enviornment and then on hardware enviornmemt(Lego Robot).

How I solved them  
- By reading manual provided with components box manage to construct the robot
- Keep the distance minimum between wheels because if the distance is bigger, it will be difficult for the robot to follow and turns on   the lines.
- I spend time to learn how to work with EV3 software building blocks and done some test with MATLAB,but EV3 is more useful just playing   with the blocks.
- I studied some manuals and I able to setup the connection between lego robot and software via bluetooth and WIFI.
- I learn how to calibrate the color sensor with 3 different functionalities.
- I tune the PID controller according to the robot stability and turns on line.

## Code Example

This project includes the EV3 software project files for line follower robot using PID Controller.

## Explanation of the Result

If the system must remain stable follows these steps 
- Initially set Kd and Ki to 0.
- Set Kp to 1 and run the robot if it is not following a straight line change it until the output of the loop oscillates and robot         follows a straight line without oscillations.
- Increase Ki until any offset is corrected in sufficient time for the process.If Ki is too much higher then it will cause instability. 
- Increase Kd, until the loop is acceptably quick to reach its reference after a load disturbance but if Kd is set too much higher it     will cause excessive response and overshoot. 

## Explanation why these values are the best

These are the best values which I got after tuning 
- Kp is 0.99
- Ki is 0.8
- Kd is 0.40
- Steering Speed is 26

These values are best because my robot is following a straight line without oscillation and follows the line accuaretly without any instability. Because Kp tells us how far the robot is from the line(i.e. to the right,to the extreme right,to the left or a little to the left). Proportional is the fundamental term used to follow the path.Ki gives the accumulated error over time and tells us if the robot has been on the line in the last few moments or not and Kd is the rate at which the robot oscillates to the left and right about the line.

## Link to youtube video (Shows movement of my robot)

- https://youtu.be/aPAZZjKmMbk (Track 1)

- https://youtu.be/6HL_vltD60Q (Track 2)

- https://youtu.be/iWL4Vnwe4DI (Track 3)

