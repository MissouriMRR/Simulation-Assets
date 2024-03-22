## ODLC Insert Object
This object will repeatedly change its texture to an assigned image.

# Getting Started

To assign a filepath, first double click on *ODLC_Blue_Blueprint* as shown in the image below.
![alt text]([ODLC_Insert_Object/README_Images/Blueprint Object.png]))

Next, change the *ODLCFile Path* string variable to the absolute path of the location of the images on your computer as shown below.
![alt text]([ODLC_Insert_Object\README_Images\Delay.png])

Unfortunetly, you cannot assign unique filepaths to multiple ODLC_Blue_Blueprint objects. To make multiple ODLC_Blue_Blueprint have unique images you must use a wildcard (*) in your filepath. 
When the program runs, the wildcard will be replaced with a number 0- # odlc objects in the file path. 

For example, if you assign *ODLCFile Path* to the filepath C:/User/image*.png then ODLC object 1 will change its texture to C:/User/image0.png, object 2 will change its texture to C:/User/image1.png and so on.

To use this blueprint to its fullest potential, you should procedurally change the images at the entered filepath using a seperate program.

This blueprint updates the texture to the image filepath every 10 seconds. To change this, double click on *ODLC_Blue_Blueprint*, expand EventGraph, double click on Event BeginPlay, and change the number in the specific blueprint node shown below.

![alt text]([ODLC_Insert_Object/"README Images"/Delay.png])

