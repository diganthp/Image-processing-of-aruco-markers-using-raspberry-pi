# Image processing of Aruco Markers using Raspberry Pi
By Dheeraj Kamath, Diganth P, Balaji and Harshith J Shiva
## Aruco Markers
ArUco markers are binary square fiducial markers that can be used for camera pose estimation. Their main benefit is that their detection is robust, fast and simple.

An ArUco marker is a synthetic square marker composed by a wide black border and a inner binary matrix which determines its identifier (id). The black border facilitates its fast detection in the image and the binary codification allows its identification and the application of error detection and correction techniques. The marker size determines the size of the internal matrix. For instance, a marker size of 4x4 is composed by 16 bits.


![alt text](https://github.com/diganthp/Image-processing-of-aruco-markers-using-raspberry-pi/blob/master/Images/aruco.png)

The first, third and fifth columns represent parity bits. The second and fourth columns represent the data bits.

## The Method Description
### Step 1: Extract the ArUco from the Image

![alt text](https://github.com/diganthp/Image-processing-of-aruco-markers-using-raspberry-pi/blob/master/Images/Capture2.PNG)

### Step 2: Remove the extra padding

![alt text](https://github.com/diganthp/Image-processing-of-aruco-markers-using-raspberry-pi/blob/master/Images/Capture3.PNG)

### Step 3: Converting the ArUco to Binary format
Divide the resulting image into a 5x5 grid and check the color in each cell of the second and fourth columns(in that order) in a top to bottom manner.

![alt text](https://github.com/diganthp/Image-processing-of-aruco-markers-using-raspberry-pi/blob/master/Images/Capture4.PNG)

### Step 4: If the color is white, write 1; else, write it 0

### Step 5: The resulting number will be in binary. Convert it into decimal
This is how the id of the marker is determined.

## Video Demo
[Image processing of ArUco markers using raspberry pi](https://www.youtube.com/watch?v=H4fQttAG27Q)
