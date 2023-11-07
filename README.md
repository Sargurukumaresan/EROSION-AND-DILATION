# EROSION-AND-DILATION

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import necessary packages

### Step2:
Create an empty window and add text to it
### Step3:
create a structuring element

### Step4:
Do the operation

### Step5:
Show the output image

 
## Program:
```
NAME:SARGURU.K
REG NO:212221230134
```

``` Python
# Import the necessary packages
import cv2
import numpy as np


# Create the Text using cv2.putText

img= np.zeros((350,1400),dtype ='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'SARGURU.K',(15,200),font,5,(255),10,cv2.LINE_AA)
cv2.imshow('created_text',img)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Create the structuring element



# Erode the image

erode1= np.ones((5,5),np.uint8)
erode2 = cv2.getStructuringElement(cv2.MORPH_CROSS,(12,12))

image_erode1 = cv2.erode(img,erode1)
cv2.imshow('Eroded_image_1',image_erode1)
cv2.waitKey(0)
cv2.destroyAllWindows()
image_erode2 = cv2.erode(img,erode2)
cv2.imshow('Eroded_image_2',image_erode2)
cv2.waitKey(0)
cv2.destroyAllWindows()


# Dilate the image


dilate1= np.ones((5,5),np.uint8)
dilate2 = cv2.getStructuringElement(cv2.MORPH_CROSS,(12,12))

image_dilate1 = cv2.dilate(img,dilate1)
cv2.imshow('Dilated_image_1',image_dilate1)
cv2.waitKey(0)
cv2.destroyAllWindows()
image_dilated2 = cv2.dilate(img,dilate2)
cv2.imshow('Dilated_image_2',image_dilated2)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
## Output:

### Display the input Image
![WhatsApp Image 2023-11-07 at 14 15 26_6df50007](https://github.com/Sargurukumaresan/EROSION-AND-DILATION/assets/119559840/c94dfacc-9a2c-4532-b57a-b103e3179ea6)




### Display the Eroded Image

![WhatsApp Image 2023-11-07 at 14 15 26_35cacc96](https://github.com/Sargurukumaresan/EROSION-AND-DILATION/assets/119559840/487bdc05-fc8f-417b-b8b3-9dfc831b54e7)



### Display the Dilated Image
![WhatsApp Image 2023-11-07 at 14 15 26_be1eab75](https://github.com/Sargurukumaresan/EROSION-AND-DILATION/assets/119559840/5f73f030-8e0c-49c7-a7db-c96809b4128f)





## Result
Thus the generated text image is eroded and dilated using Python and OpenCV.
