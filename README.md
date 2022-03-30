
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
# Developed By: BALAJI N
# Register Number 212220230006
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



![212220230006_kakashi_hatake 29-03-2022 22_20_18](https://user-images.githubusercontent.com/75234946/160758934-a43b7de2-d585-4f91-aef5-ae0307e321e9.png)





### ii)Write the image


![Untitled144 - Jupyter Notebook - Google Chrome 29-03-2022 22_26_23](https://user-images.githubusercontent.com/75234946/160759193-a8b4b147-6e2b-463c-9fce-e555d2f57fa6.png)


### iii)Shape of the Image


![j4](https://user-images.githubusercontent.com/75234946/160673299-4855759b-8019-4106-a08d-c943d27fc558.png)


### iv)Access rows and columns



![kakashi_coloured 29-03-2022 22_23_16](https://user-images.githubusercontent.com/75234946/160759975-80cda2d3-87d7-4cf0-ab68-5bc0f559cd9b.png)




### v)Cut and paste portion of image

![Screenshot (13)](https://user-images.githubusercontent.com/75234946/160759783-5ea84dbf-005e-472e-96e1-fa17135111d5.png)




### vi)grey image

![212220230006_kakashi_hatake 30-03-2022 08_14_22](https://user-images.githubusercontent.com/75234946/160759562-e0175813-5912-4e8b-aa33-23e99099e90f.png)



## Result:
Thus the images are read, displayed, and written successfully using the python program.


