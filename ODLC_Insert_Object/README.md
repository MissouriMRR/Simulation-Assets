## ODLC Insert Object 

This object will repeatedly change its texture to an assigned image. 

  

# Getting Started 

  

To assign a file path, first double click on *ODLC_Blue_Blueprint* as shown in the image below. 

  

![](https://github.com/MissouriMRR/Simulation-Assets/blob/bad632e45b052fc2e005902d679fe30278f64913/ODLC_Insert_Object/README_Images/Blueprint%20Object.png) 

  

Next, change the *ODLCFile Path* string variable to the absolute path of the location of the images on your computer as shown below. 

  

![](https://github.com/MissouriMRR/Simulation-Assets/blob/bad632e45b052fc2e005902d679fe30278f64913/ODLC_Insert_Object/README_Images/Filepath%20String.png) 

  

Unfortunately, you cannot assign unique file paths to multiple ODLC_Blue_Blueprint objects. To make multiple ODLC_Blue_Blueprint have unique images you must use a wildcard (*) in your file path.  

When the program runs, the wildcard will be replaced with a number 0- # odlc objects in the file path.  

  

For example, if you assign *ODLCFile Path* to the file path C:/User/image*.png then ODLC object 1 will change its texture to C:/User/image0.png, object 2 will change its texture to C:/User/image1.png and so on. 

  

To use this blueprint to its fullest potential, you should procedurally change the images at the entered file path using a separate program. 

  

This blueprint updates the texture to the image file path every 10 seconds. To change this, double click on *ODLC_Blue_Blueprint*, expand EventGraph, double click on Event BeginPlay, and change the number in the specific blueprint node shown below. 

![](https://github.com/MissouriMRR/Simulation-Assets/blob/8fd19ae7d02ae46970efe0b6a5525929374e2988/ODLC_Insert_Object/README_Images/Delay.png) 

 

 
