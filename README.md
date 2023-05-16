## Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
## Step1:
Import necessary packages

## Step2:
Create a empty window and add text in it

## Step3:
Create a structuring element

## Step4:
Do the operation

## Step5:
Do the operation
## Program:
## Developed By:S.ABHISHEK
## Register No:212221230002
## Import the necessary packages
```

import cv2
import numpy as np
import matplotlib.pyplot as plt

```

## Create the Text using cv2.putText
```
img1=np.zeros((100,660),dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX = 3
cv2.putText(img1,'S.ABHISHEK',(130,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1,'gray')
plt.axis('off')
```


## Create the structuring element
```

kernel=np.ones((5,5),np.uint8)


```
## Erode the image
```

image_erode1=cv2.erode(img1,kernel)
plt.imshow(image_erode1,'gray')
plt.axis('off')

```

## Dilate the image
```
image_dilatel=cv2.dilate(img1,kernel)
plt.imshow(image_dilatel,'gray')
plt.axis('off')
```
## Output:

## Display the input Image
![image](https://github.com/S-ABHISHEK-1905/Implementation-of-Erosion-and-Dilation/assets/66360846/9221c6ae-9456-4cdb-bc1a-5297a6c9a2e1)


## Display the Eroded Image
![image](https://github.com/S-ABHISHEK-1905/Implementation-of-Erosion-and-Dilation/assets/66360846/46239357-2bf3-4e01-b767-9e932e752722)

## Display the Dilated Image
![image](https://github.com/S-ABHISHEK-1905/Implementation-of-Erosion-and-Dilation/assets/66360846/4b972964-4c88-4b9e-b4d0-1b3ab3df76cc)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
