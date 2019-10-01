# Drowning-Detector
Using YOLO object detection, this program will detect if a person is drowning. This software can be used with a Raspberry Pi Camera, which can then be placed underwater with an appropiate case.

The approach to this project is to first detect a person, drawing a blue rectangle around them. The program will now store the centre of that rectangle (the person's) position, and compare it to the person's position is more or less the same or they are falling, and this continues for 10 seconds, the blue rectangle will now turn red and the word 'DROWNING' will appear on top of it.

If the person´s centre is above water, the word ´DROWNING´ will be removed as they are just standing in the pool. 

Doing some research, I discovered that when someone drowns, they tend to stay in a vertical position to try to keep their head above water level. This could be analysed by seeing the ratio of height to width of the triangle to determine if the person is vertically (drowning) or horizontally (swimming or diving) positioned.

This project was developed by AI Society at CLS, with the aim to help the lifeguards in the school´s swimming pool. 

To install the necessary packages, run

pip install -r requirements.txt

If you are interested in YOLO object detection, read their website:

https://pjreddie.com/darknet/yolo/
