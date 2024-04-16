# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>Import the necessary packages


### Step2:
<br>Create the Text using cv2.putText

### Step3:
<br>Create the structuring element

### Step4:
<br>Erode the image

### Step5:
<br>Dilate the image

### Step6:
Display the output images

 
## Program:
Eroding 
``` python
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Engineer',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image_erode1=cv2.erode(img1,kernel1)
plt.imshow(image_erode1)
plt.axis("off")
```

```python
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Engineer',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image_dilate1=cv2.dilate(img1,kernel1)
plt.imshow(image_dilate1)
plt.axis("off")

```
## Output:

### Display the input Image
<br>![image](https://github.com/MeethaPrabhu/erosion-dilation/assets/119401038/69e0e823-0e09-4e67-8018-cafe7de0e979)

<br>
<br>
<br>
<br>
<br>

### Display the Eroded Image
<br>![image](https://github.com/MeethaPrabhu/erosion-dilation/assets/119401038/af10c9ed-d69a-47e6-a7f9-37245ea42524)

<br>
<br>
<br>
<br>
<br>

### Display the Dilated Image
<br>![image](https://github.com/MeethaPrabhu/erosion-dilation/assets/119401038/6e40d034-8417-4956-b233-a0bd90a989f2)

<br>
<br>
<br>
<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
