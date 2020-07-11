![Alt Text](https://media.giphy.com/media/kdXnsLKl3mMLG1kuuw/giphy.gif)

# Raspberry-Pi-Facial-Recognition-w-GUI

Using Python, OpenCV and a Raspberry Pi, I created a program that lets you add photos of a person, and the Raspberry Pi will detect their face.


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

**Installing OpenCV**
This website is the best <a href="https://www.pyimagesearch.com/2019/09/16/install-opencv-4-on-raspberry-pi-4-and-raspbian-buster/">with explaing in great detail how to install OpenCV on your Raspberry Pi.</a> 

**Getting the Program started**
Now that
