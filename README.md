# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By: DHARSHINI.D.S
### Register Number: 212221230022
i) #To Read,display the image
```
import cv2
A=cv2.imread("img1.png",1)
cv2.imshow("Dharshini.DS",A)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
A=cv2.imread("img1.png",1)
cv2.imshow("Dharshini.DS",A)
cv2.waitKey(0)

```
iii) #Find the shape of the Image
```
import cv2
color_image = cv2.imread('img1.png',1)
print(color_image.shape)


```
iv) #To access rows and columns

```
import random
import cv2
A=cv2.imread("img1.png",1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212221230022",A)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```
import cv2
color_image = cv2.imread('img1.png',1)
part = color_image[300:400,300:400]
color_image[50:150,50:150] = part
cv2.imshow("dharshini.ds",color_image)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image
![exp 1 a ds](https://user-images.githubusercontent.com/93427345/225527081-216e7b15-f847-48a2-ad19-6450a8ad1e15.png)


### ii)Write the image
![exp 1 a ds](https://user-images.githubusercontent.com/93427345/225527186-1eb9b612-6c17-4638-81eb-df120c81a3a3.png)


### iii)Shape of the Image

![exp 1b ds](https://user-images.githubusercontent.com/93427345/225527269-bb8930f2-db73-497c-943d-a43f01f9328f.png)


### iv)Access rows and columns

![exp1c ds](https://user-images.githubusercontent.com/93427345/225527308-273744b9-a63b-4772-9088-4a7b16b21a41.png)

### v)Cut and paste portion of image
![exp 1d ds](https://user-images.githubusercontent.com/93427345/225527363-8ee50091-3e91-45e1-b318-2ee824fdd548.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


