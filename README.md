# ekfmonoslam

SLAM based on EKF using a monocular camera, optionally an IMU, and GPS data. This package has been tested in matlab 2012 on 64bit Windows 8.1. 

Before running sample tests, a few packages need to be downloaded. To begin with, create a folder to contain all the related packages, e.g., matlab_ws.

#1. Dependencies

##1.1 1-Point RANSAC Inverse Depth EKF Monocular SLAM v1.01

You can download the package from http://webdiis.unizar.es/~jcivera/code/1p-ransac-ekf-monoslam.html. Extract the package, and put the EKF_monoSLAM_1pRANSAC folder into matlab_ws. Note this package contains an example sequence. Change the name of the subfolder /EKF_monoSLAM_1pRANSAC/matlab_code/@ekf_filter into /EKF_monoSLAM_1pRANSAC/matlab_code/ekf_filter

##1.2 Camera calibration toolbox for matlab

From this web page http://www.vision.caltech.edu/bouguetj/calib_doc/, search for "download page", then download the package and extract and put it into matlab_ws, too.

##1.3 MexOpenCV and OpenCV

It can be forked or downloaded from https://github.com/kyamagu/mexopencv. Also, extract and put mexopencv into matlab_ws folder. Compile the mex files according to the instructions on https://github.com/kyamagu/mexopencv.

##1.4 INS toolkit (included)

ekfmonoslam also depends on the INS toolkit which can be found at http://www.instk.org/. Since I made much changes to instk, I included it in ekfmonoslam package.

#2. Build

Download the ekfmonoslam package, put all folders within ekfmonoslam into matlab_ws. Because there is a EKF_monoSLAM_1pRANSAC folder in this package which contains patches to 1-Point RANSAC Inverse Depth EKF Monocular SLAM v1.01, you may be prompted to replace or merge files, replace these files already in matlab_ws.

#3. Test with Data

Test data due to size will be made available upon request.



