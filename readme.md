# Temporal matching prior network
Temporal matching prior network for license plate detection and recognition in videos, in review.

# Results
[![Demo](https://user-images.githubusercontent.com/46806852/56007668-6bc03b00-5d14-11e9-9f93-1077caf93340.PNG)](https://github.com/seokbongyoo/Dataset_for_LPR/blob/master/%5BDemo_video%5DCaltech_plate_detection.mp4)

<iframe width="1488" height="1012" src="https://github.com/seokbongyoo/Dataset_for_LPR/blob/master/%5BDemo_video%5DCaltech_plate_detection.mp4" frameborder="0" allowfullscreen></iframe>

PlateDetection Executable made by Seok Bong Yoo

1. Prerequisites for Deployment 

High-performence GPU, CUDA 9.1, and CUDNN 7.1.3 are required.

https://developer.nvidia.com/cuda-toolkit-archive 
https://developer.nvidia.com/rdp/cudnn-archive

Verify that version 9.3 (R2017b) of the MATLAB Runtime is installed.   

If the MATLAB Runtime is not installed, you can run the MATLAB Runtime installer.
To find its location, enter
  
    >>mcrinstaller
      
at the MATLAB prompt.

Alternatively, download and install the Windows version of the MATLAB Runtime for R2017b 
from the following link on the MathWorks website:

    http://www.mathworks.com/products/compiler/mcr/index.html
   
For more information about the MATLAB Runtime and the MATLAB Runtime installer, see 
Package and Distribute in the MATLAB Compiler documentation  
in the MathWorks Documentation Center.    

NOTE: You will need administrator rights to run the MATLAB Runtime installer. 


2. Files to Deploy and Package

Files to Package for Standalone 
================================
-PlateDetection.exe
-MCRInstaller.exe 
    Note: if end users are unable to download the MATLAB Runtime using the
    instructions in the previous section, include it when building your 
    component by clicking the "Runtime downloaded from web" link in the
    Deployment Tool.
-This readme file 

3. Definitions

For information on deployment terminology, go to
http://www.mathworks.com/help and select MATLAB Compiler >
Getting Started > About Application Deployment >
Deployment Product Terms in the MathWorks Documentation
Center.

4. Execution

- Decompress egg files in model folder(model/).
- Locate model.weight file in model folder(model/).
- Locate test images in input folder(Caltech/images/).
- Write the position of each image in Caltech_images.txt.
- Run Test.cmd.
- Confirm many plate detection results by pressing any key in keyboard.


