# PAN-Card-Tampering-Detection #

UCS757 - Building Innovative Systems <br>
Project - 1 <br>

## Overview: ##
The purpose of this project is to detect tampering of PAN card using computer vision. This project will help different organization in detecting whether the Id i.e. the PAN card provided to them by thier employees or customers or anyone is original or not.

### Methodology : <br/> ###
![1_SBVkh54RJZrMsozG-vQdCQ](https://user-images.githubusercontent.com/48948891/134335724-93e8100e-0c52-4b9e-a1e9-0372769d1eb5.png)<br>

● Loading original and user provided images.<br>

● Converting the format of tampered image similar to original image.<br>

● Checkeing the format and size of the original and tampered image.<br>

● Converting the size of tampered and original image.<br>

● Converting images into grayscale using opencv. Because in image processing many applications doesn't help us in identifying the important, edges of the coloured images also coloured images are bit complex to understand by machine beacuse they have 3 channel while grayscale has only 1 channel.<br>

● Structural similarity index helps us to determine exactly where in terms of x,y coordinates location, the image differences are. Here, we are trying to find similarities between the original and tampered image. The lower the SSIM score lower is the similarity.<br>

● Next we are using the threshold function of computer vision which applies an adaptive threshold to the image which is stored in the form array. This function transforms the grayscale image into a binary image using a mathematical formula.<br>

● Bounding rectangle helps in finding the ratio of width to height of bounding rectangle of the object. We compute the bounding box of the contour and then draw the bounding box on both input images to represent where the two images are different or not.<br>

● Finally we visualized the differences and similarities between the images using by displaying the images with contours, difference and threshold.<br>

### Live Link: https://pancard-tampering-1.herokuapp.com/ ###
(Sample Data already enclosed in this github-repo)

### I/O Screenshot :<br/> ###
#### Input-1 (Original) ####
![original](https://user-images.githubusercontent.com/48948891/133932760-89f3f757-5551-4511-bc8b-7ecdc1397017.jpg)
<br>
![Screenshot (441)](https://user-images.githubusercontent.com/48948891/133932572-638b9c11-35b9-4d90-828f-421ce5624fea.png)
</br>
Output-1
![Screenshot (442)](https://user-images.githubusercontent.com/48948891/133932650-c126736b-77b7-4377-8e77-d755f3d939ba.png)
</br>
#### Input-2(Tampered) ####
![tampered](https://user-images.githubusercontent.com/48948891/133932765-19ee7aed-168e-4e10-b9f2-1ce5f4501c3f.jpg)
</br>
![Screenshot (443)](https://user-images.githubusercontent.com/48948891/133932678-064446c2-2f53-4188-89e0-9fac0302bb71.png)
</br>
Output-2
![Screenshot (444)](https://user-images.githubusercontent.com/48948891/133932696-8274d7ad-19ba-47f5-b7bb-55c73b9046b0.png)
</br>
### Summary :<br/> ###

-Finding out structural similarity of the images helped us in finding the difference or similarity in the shape of the images. Similarly, finding out the threshold and contours based on those threshold for the images converted into grayscale binary also helped us in shape analysis and recognition.<br>

-As, our SSIM is ~28.5% we can say that the image user provided is fake or tampered.<br>

### Novelty :<br/> ###
●	This project can be used in different organizations where customers or users need to provide any kind of id in order to get themselves verified.<br>

● The organization can use this project to find out whether the ID is original or fake. Similarly this can be used for any type of ID like adhar, voter id, etc.<br>



