# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
## Step1:
Import the necessary packages

## Step2:
Create the Text using cv2.putText

## Step3:
Create the structuring element

## Step4:
Use Opening operation

## Step5:
Use Closing Operation
 
## Program:

## Display the input Image
```python
import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'ICE AGE', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)
```
## Create ths structured element
```python
struct_ele = np.ones((9, 9), np.uint8)
```
## Display the result of Opening
```python
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
## Display the result of Closing
```python
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:
## Display the input Image
![image](https://github.com/KothaiKumar/OPENING--AND-CLOSING/assets/121215739/85cd5a5f-1339-4c90-be9b-85aaa9efff99)
## Display the result of Opening
![image](https://github.com/KothaiKumar/OPENING--AND-CLOSING/assets/121215739/9fe06009-fb18-4b68-98f7-259b8834283e)
## Display the result of Closing
![image](https://github.com/KothaiKumar/OPENING--AND-CLOSING/assets/121215739/afc67416-971c-40ad-ad94-ff77aec1894f)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
