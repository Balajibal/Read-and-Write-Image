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
```python
# Developed By:
# Register Number
# To Read,display the image
import cv2
img = cv2.imread('kakashi-hatake-wallpaper-hd-1366x768-396324.jpg',1)
cv2.imshow('212220230006_kakashi_hatake',img)
cv2.waitKey(0)



# To write the image
cv2.imwrite('download.jpg',img)





# Find the shape of the Image
print(img.shape)




# To access rows and columns
import random
for i in range(200):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('kakashi_coloured',img)
cv2.waitKey(0)





# To cut and paste portion of image
img1 = cv2.imread('kakashi-hatake-wallpaper-hd-1366x768-396324.jpg',1)
tag = img1[300:400:,300:400]
img1[50:150,50:150] = tag
cv2.imshow('img',img1)
cv2.waitKey(0)



# grey image
grey = cv2.imread('kakashi-hatake-wallpaper-hd-1366x768-396324.jpg',0)
cv2.imshow('212220230006_kakashi_hatake',img)
cv2.waitKey(0)










```
## Output:

### i) Read and display the image

<br>

![j2](https://user-images.githubusercontent.com/75234946/160672959-43bdab85-bab9-429c-b80b-ba00f71699b5.jpeg)

<br>


### ii)Write the image

<br>
![j3](https://user-images.githubusercontent.com/75234946/160673009-d99220bb-8978-46fa-8cee-fbff2813c926.jpeg)
<br>
### iii)Shape of the Image

<br>
![j4](https://user-images.githubusercontent.com/75234946/160673299-4855759b-8019-4106-a08d-c943d27fc558.png)
<br>


### iv)Access rows and columns
<br>


![j5](https://user-images.githubusercontent.com/75234946/160673409-22686314-5bb5-431b-9e43-e884dd222916.jpeg)
<br>


### v)Cut and paste portion of image
<br>
![j6](https://user-images.githubusercontent.com/75234946/160673587-6305098f-dd5c-410a-bd05-5813fbf6fdf0.jpeg)
<br>


### vi)grey image
<br>
![j1](https://user-images.githubusercontent.com/75234946/160673663-a688a871-76bb-4b6b-8ab1-83191b0910f7.jpeg)
<br>


## Result:
Thus the images are read, displayed, and written successfully using the python program.


