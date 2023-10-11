# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step 1 :
Import the necessary packages.

## Step 2 :
Create the Text using cv2.putText

### Step 3 :
Create the structuring element.

### Step 4 :
Use Opening operation.

### Step 5 :
Use Closing Operation.

## Program:
## DEVELOPED BY :NIROSHA S
## REGISTER NO : 212222230097
## Import the necessary packages :
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
## Create the Text using cv2.putText :
```
img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img,'ABRIN NISHA',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img)
plt.show()
```
## Create the structuring element :
```
kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(9,9))
```
## Use Opening operation :
```
image_open=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.axis('off')
plt.imshow(image_open)
plt.show()
```
## Use Closing Operation :
```
image_close=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.axis('off')
plt.imshow(image_close)
plt.show()
```
## Output :
## Display the input Image :
![image](https://github.com/Niroshassithanathan/OPENING--CLOSING/assets/121418437/fe04d1d6-1f53-4cb8-a71a-bb0fd5a85ea0)

## Display the result of Opening :
![image](https://github.com/Niroshassithanathan/OPENING--CLOSING/assets/121418437/0a903a22-4474-424b-9c40-e61c66548ea6)

## Display the result of Closing :
![image](https://github.com/Niroshassithanathan/OPENING--CLOSING/assets/121418437/46676eb5-061f-42b0-80ae-bb1e4e0261ae)

## Result :
Thus the Opening and Closing operation is used in the image using python and OpenCV.


