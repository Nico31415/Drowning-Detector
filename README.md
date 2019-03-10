# Drowning-Detector
Using YOLO object detection, this program will detect if a person is drowning. This project is still a work in progress, so it can only be implemented with a computer's webcam, and doesn't work completely yet.

The approach to this project is to first detect a person, drawing a blue rectangle around them. The program will now store the centre of that rectangle (the person's) position, and compare it to the person's position is more or less the same or they are falling, and this continues for 5 seconds, the blue rectangle will now turn red and the word 'DROWNING' will appear on top of it.

Necessary packages:

cvlib (included in commit)
numpy (pip install numpy)
opencv (pip install opencv-python)
