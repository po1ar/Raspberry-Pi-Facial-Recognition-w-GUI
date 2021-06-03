![Alt Text](https://media.giphy.com/media/kdXnsLKl3mMLG1kuuw/giphy.gif)

# Raspberry-Pi-Facial-Recognition-w-GUI

Using Python, OpenCV and a Raspberry Pi, I created a program that lets you add photos of a person, and the Raspberry Pi will detect their face.

![alt text](https://media.giphy.com/media/eIyieq01EAYkQS7qsB/giphy.gif)

## Materials:
- Raspberry Pi (used 4b for this project)
- Pi Camera Module (used v2.1)
- SD Card w/Raspbian/PiOS

**Optional:**
- LCD Display

## Installation:

First, make sure the camera module is connected AND YOU ENABLED I2C. To check, run this command on terminal 

```
vcgencmd get_camera
```
If the response is:
```
supported=1 detected=1
```
then your camera is all ready! Onto the next step.

## Installing OpenCV 
This website is the best <a href="https://www.pyimagesearch.com/2019/09/16/install-opencv-4-on-raspberry-pi-4-and-raspbian-buster/">with explaing in great detail how to install OpenCV on your Raspberry Pi.</a> 

## Getting All The Files 
Now that OpenCV is installed, clone this repo with
```
git clone https://github.com/po1ar/Raspberry-Pi-Facial-Recognition-w-GUI.git
```
Then, install all the libraires needed for this project
```
$ pip3 install dlib  
$ pip3 install face_recognition  
$ pip3 install imutils
```
## Running The Program
**Step 1:**
To run the first program open termianl and enter
```
$ python3 faceDataset.py 
```
After running it, you should see a pop-up like this:

![alt text](https://media.giphy.com/media/QBpSHY3JPTcgTb7YSn/giphy.gif)

Enter the name of the person that is in the photos. If the name is not entered, the folder will not be created. This is the folder where all the images of that person will be stored and is required for further processing.

An image capturing window will open. Click on Snapshot to take the photos. It will store a single image every time you click on Snapshot. Take at least 6-7 images in the different face position, for example straight, tilt and side pictures. Close the window when done.

![alt text](https://media.giphy.com/media/QTxt4wb68v4W9zIOqN/giphy.gif)

To create multiple people, repeat the steps.

**NOTE:** If numerous person data are stored, the encoding time will increase, as the raspberry pi is a low power computer it will take more time to process, and the facial recognition will run slower.

**Step 2:**
Run the Facial Recognition file with:
```
$ python3 face_recognize.py 
```
After running a window will pop up like this:

![alt text](https://media.giphy.com/media/UTf13jj0liZYTLf451/giphy.gif)

After processing the images, the "Frame window" will open, when the camera detects the person's face, it will show the name of the person if its matches with the images in the database. Press Q on the keyboard to close the Frame window.

Congrats! You have built a Facial Recognition Camera with the Raspberry Pi.

## Credits: 
First off, thank you to <a href="https://hackclub.com"> Hack Club </a> for making this project a possibility. Also, full credit and a big thank you to Sharib Hasan for creating most of the code for this project. 

## Contact: 
If you have any questions about this project my email is danielanapolsky@gmail.com

---------------------------------------
Thanks for checking my project out!

