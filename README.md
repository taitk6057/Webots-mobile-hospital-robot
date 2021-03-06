# ECE183DB

Robotic automation simulation for an autonomously line-follow to transport linens for nurses at chosen stop points tailored to any hospital. 

Our controller begins with the simple robot structure definitions like the motor and sensor lists. This is followed by the error definitions and PID function. Then while the simulation is running, depending on the track and corresponding sensor readings, we will either navigate according to line following or edge following. Each reads in live sensor values and sets the correct motor speed for each of the drive wheels. Then we run the main loop where depending on particular sensor readings and obstacles, we execute one of the modes from the diagram above. There are modes for starting, line following when there are no obstacles and the IR values indicate a white line with black outer track, edge following when the left and right IR sensors pick up different contrasting values (black and white on opposite sides, not black on both sides), obstacle modes and stopping conditions. 

Here is the final webots controller and one of our corresponding simulation worlds for testing
