# Opening-and-Closing

## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
## Step 1:
Import the necessary packages.

## Step 2:
Create the Text using cv2.putText.

## Step 3:
Create the structuring element.

## Step 4:
Use Opening operation.

## Step 5:
Use Closing Operation.

 
## Program:

Developed by: P.SYAM TEJ.
Regestration no:212221240056.

``` Python
# Import the necessary packages
import numpy as np
import cv2
import matplotlib.pyplot as plt
# Create the Text using cv2.putText
img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL
im=cv2.putText(img1,' AmarNath ',(5,70),font,2,(255),5,cv2.LINE_AA)
# Create the structuring element
Kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(11,11))
# Use Opening operation
image1=cv2.morphologyEx(im,cv2.MORPH_OPEN,Kernel)
plt.imshow(image1)
# Use Closing Operation
image1=cv2.morphologyEx(im,cv2.MORPH_CLOSE,Kernel)
plt.imshow(image1)

```
## Output:

### Display the input Image

![11 1](https://user-images.githubusercontent.com/93427224/172896715-4967f4d5-09cd-416b-830e-8caa4a3e2c27.png)

### Display the result of Opening

![11 2](https://user-images.githubusercontent.com/93427224/172896740-001f69db-f221-4fbc-b320-21b5b5bbac0d.png)

### Display the result of Closing

![11 3](https://user-images.githubusercontent.com/93427224/172896779-749d0ca2-c4c0-4db0-99e4-acb901361db3.png)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
