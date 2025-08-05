I made this because the adafruit library uses circuit python and I didn't want to. 
I used micropython to program it.
One issue I kept coming up with was that the first register for the Z axis never really
changed.
Not sure if I'm unpacking the registers incorrectly or my one is just broken
The temperature sensor works well though

I have only implemented it for the z axis but if you wanted, you can literally just copy
and paste it and just change the registers for it. That's literally it
The registers are written in comments in the library or you can look at the datasheet

If someone wants to take this and improve it, be my guest. 

if ((len(status_binary) >= 10) and (int(status_binary[len(status_binary)-(1+6)]) == 1)):#reading magnetic field
This really weird line and the line below that which is similar is just to check
if the magnetometer is ready to have the data read

Good luck :D
