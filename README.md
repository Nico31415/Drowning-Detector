# Drowning-Detector
Using YOLO object detection, this program will detect if a person is drowning. This project is still a work in progress, so it can only be implemented with a computer's webcam, and doesn't work completely yet.

The approach to this project is to first detect a person, drawing a blue rectangle around them. The program will now store the centre of that rectangle (the person's) position, and compare it to the person's position is more or less the same or they are falling, and this continues for 10 seconds, the blue rectangle will now turn red and the word 'DROWNING' will appear on top of it.

Doing some research, I discovered that when someone drowns, they tend to stay in a vertical position to try to keep their head above water level. This could be analysed by seeing the ratio of height to width of the triangle to determine if the person is vertically (drowning) or horizontally (swimming or diving) positioned.

To install the necessary packages, run

pip install -r requirements.txt

If you are interested in YOLO object detection, read their website:

https://pjreddie.com/darknet/yolo/
