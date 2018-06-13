# Image processing of Aruco Markers using Raspberry Pi

## Aruco Markers
ArUco markers are binary square fiducial markers that can be used for camera pose estimation. Their main benefit is that their detection is robust, fast and simple.

An ArUco marker is a synthetic square marker composed by a wide black border and a inner binary matrix which determines its identifier (id). The black border facilitates its fast detection in the image and the binary codification allows its identification and the application of error detection and correction techniques. The marker size determines the size of the internal matrix. For instance, a marker size of 4x4 is composed by 16 bits.
![alt text](https://github.com/diganthp/Image-processing-of-aruco-markers-using-raspberry-pi/blob/master/Images/aruco.png)
