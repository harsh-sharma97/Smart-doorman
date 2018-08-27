# Smart-doorman
IOT based MDD project
Before the use of  smart lock system



 1.  you could not supervise your home if you were
out.



 2.  you needed to be physically present to unlock
your home



 3.  you could not keep track who enters or exits your
home.



 4.  burglary was widely possible.



After



- All the things stated above
are now possible by using actuators and sensors and other computation methods.

These exist few products in area of smart locking system but most of
them are in collaboration with the smart home package which costs a fortune. Moreover
adding these edits will make it widely usable.



Edits:

1)Introducing doorbells that
give notification on your smartphone rather than ringing out loud at homes or
in fact doing both will be very effective as we tend to be closer to our mobile
phones than our partners nowadays.
2)changing the security key for
the lock on a daily basis could be one possible attempt to ensure security.


Drawback:
If one gets the access to the remote , that is the users cell phone he will be out in
the open. the price godrej charges is around 20,000+ for full setup. originally
there were no such atribute just a lock and a doorbell costing around 4-5k rs.
now with the aided benefits anyone will be willing to spend a decent amount on
their security.



 Basic implementation and familiarity with Arduino


Required components:



 1.  Arduino uno


2. Jumper wires



-these are used for pin to pin connections between arduino ,breadboard ,
sensor and buzzers.

 3. Piezo buzzer



- used as an alarming medium, it
works by continuous movement of magnet using elecromagnetic induction. When
current is passed the magnet vibrates at a certain frequency producing
sound/light.

4. PIR


For presence detection Module has two outputs:



 1.        AO, analog output, real-time output voltage signal of
the PIR sensor



 2.        DO, when the PIR sensor reaches a certain threshold,
the output high and low signal



The threshold-sensitivity can be adjusted
via potentiometer on the sensor.




Connecting to arduino



Pin + to Arduino 5+



 Pin - to Arduino -



 Pin A0 to Arduino A0 (for analog program)



 Pin D0 to Arduino 13 (for digital program)


the longer terminal of buzzer/led should
be connected to aruino +ve and the shorter one to the ground. 



The given code snippet was written to make
the coding segment under arduino programming for presence detection.


Working of this Project is very simple. A PIR sensor is used to detect the presence of any person and a Pi Camera is used to capture the images when the presence it detected.

Whenever anyone or intruder comes in range of PIR sensor, PIR Sensor triggers the Camera through aurdiuno. aurduino sends commands to  camera to click the picture and save it. After it, Aurduino creates a mail and sends it to the defined mail address with recently clicked images. The mail contains a message and picture of intruder as attachment. Here we have used the message “Please find the attachment”, you can change it accordingly in the Code .

 

Here the pictures are saved in Raspberry Pi with the name which itself contains the time and date of entry. So that we can check the time and date of intruder entry by just looking at the Picture name, check the images below. 


