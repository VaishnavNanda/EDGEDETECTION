# EDGEDETECTION

## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import the required packages for further process.
<br>


### Step2:
Read the image and convert the rgb image to gray scale image.
<br>

### Step3:
Use filters for smoothing the image to reduce the noise.
<br>

### Step4:
Apply the respective filters - Sobel, Laplacian edge detector and Canny edge detector.
<br>

### Step5:
Display the filtered image using plot and imshow.
<br>

 
## Program:
DEVELOPED BY : JEEVAGOWTHAM S
REG NO: 212222230053


# Import the packages:
```
import cv2
import matplotlib.pyplot as plt
image = cv2.imread("porsche.jpeg")
gray_image = cv2.cvtColor(image,cv2.COLOR_BGR2GRAY)
new_image = cv2.GaussianBlur(gray_image,(3,3),0)
```



# Load the image, Convert to grayscale and remove noise



# SOBEL EDGE DETECTOR:
# sobel x;
```
sobelx = cv2.Sobel(new_image,cv2.CV_64F,1,0,ksize = 5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(new_image,cmap = 'gray')
plt.title('gray')
plt.subplot(1,2,2)
plt.imshow(sobelx,cmap = 'gray')
plt.title("Sobel X")
plt.xticks([])
plt.yticks([])
plt.show()
```
# sobel y;
```
sobely = cv2.Sobel(new_image,cv2.CV_64F,0,1,ksize = 5)
plt.figure(figsize = (8,8))
plt.subplot(1,2,1)
plt.imshow(new_image,cmap = 'gray')
plt.title('gray')
plt.subplot(1,2,2)
plt.imshow(sobely,cmap = 'gray')
plt.title("Sobel Y")
plt.xticks([])
plt.yticks([])
plt.show()
```
# sobel xy;
```
sobelxy = cv2.Sobel(new_image,cv2.CV_64F,1,1,ksize=5)
plt.figure(figsize = (8,8))
plt.subplot(1,2,1)
plt.imshow(new_image,cmap = 'gray')
plt.title('gray')
plt.subplot(1,2,2)
plt.imshow(sobelxy,cmap = 'gray')
plt.title('Sobel XY')
plt.xticks([])
plt.yticks([])
plt.show()
```




# LAPLACIAN EDGE DETECTOR:
```
laplacian = cv2.Laplacian(new_image,cv2.CV_64F)
plt.figure(figsize = (8,8))
plt.subplot(1,2,1)
plt.imshow(new_image,cmap = 'gray')
plt.title('gray')
plt.subplot(1,2,2)
plt.imshow(laplacian,cmap = 'gray')
plt.title('Laplacian')
plt.xticks([])
plt.yticks([])
plt.show()
```




# CANNY EDGE DETECTOR:
```
canny_edge = cv2.Canny(new_image,120,150)
plt.figure(figsize = (8,8))
plt.subplot(1,2,1)
plt.imshow(new_image,cmap = 'gray')
plt.title('gray')
plt.subplot(1,2,2)
plt.imshow(canny_edge,cmap = 'gray')
plt.title('Canny Edges')
plt.xticks([])
plt.yticks([])
plt.show()

```



## Output:
### SOBEL EDGE DETECTOR:
# sobel x;

![Screenshot 2023-09-27 113250](https://github.com/JeevaGowtham-S/EDGEDETECTION/assets/118042624/cc026060-b934-46a0-ad5f-6a94818914f3)


# sobel y;
![Screenshot 2023-09-27 113211](https://github.com/JeevaGowtham-S/EDGEDETECTION/assets/118042624/a6032105-3a4b-4f32-b32a-72cde2d027b8)

# sobel xy;
![Screenshot 2023-09-27 113147](https://github.com/JeevaGowtham-S/EDGEDETECTION/assets/118042624/978289fd-c2fa-46c6-a76c-377271cc53b7)



<br>
<br>
<br>
<br>
<br>
<br>


### LAPLACIAN EDGE DETECTOR
![Screenshot 2023-09-27 113007](https://github.com/JeevaGowtham-S/EDGEDETECTION/assets/118042624/18dbe7bb-cd54-477c-a644-d8562971c1f1)


<br>
<br>
<br>
<br>
<br>


### CANNY EDGE DETECTOR
![Screenshot 2023-09-27 112857](https://github.com/JeevaGowtham-S/EDGEDETECTION/assets/118042624/2eabac02-5bd4-4f13-aee9-eeb088b14a0b)

<br>
<br>
<br>
<br>
<br>
<br>

## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
