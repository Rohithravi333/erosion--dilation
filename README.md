# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages

### Step2:
Create the text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Erode the image

### Step5:
Dilate the Image

## Program:
```
NAME: ROhith
REG NO: 212222230121
```
### Import the necessary packages
``` Python

import numpy as np
import cv2
import matplotlib.pyplot as plt
```

### Create the Text using cv2.putText
``` Python
img = np.zeros((100,400),dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'Rohith',(40,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img)
plt.axis('off')
```
### Create the structuring element
``` Python
kernel = np.ones((5,5),np.uint8)
kernel1 = cv2.getStructuringElement(cv2.MORPH_CROSS,(5,5))
```
### Erode the image
``` Python
img_erode = cv2.erode(img,kernel1)
plt.imshow(img_erode)
plt.axis('off')
```
### Dilate the image
``` Python
img_dilate = cv2.dilate(img,kernel1)
plt.imshow(img_dilate)
plt.axis('off')
```
## Output:

### Display the input Image

![Screenshot 2024-05-08 000530](https://github.com/Rohithravi333/erosion--dilation/assets/119394126/d32697cb-c88a-4355-9480-5568c175a43a)


### Display the Eroded Image

![Screenshot 2024-05-08 000638](https://github.com/Rohithravi333/erosion--dilation/assets/119394126/8958af0d-580a-470a-8c55-f01b6cc93c07)

### Display the Dilated Image
![Screenshot 2024-05-08 000711](https://github.com/Rohithravi333/erosion--dilation/assets/119394126/e280132e-c15e-421e-a899-982b1757d738)



## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
