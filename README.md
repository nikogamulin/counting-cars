# counting-cars
Counting cars with Movidius NCS2 and Raspberry Pi

## Counting cars with OpenVINO running on Raspberry Pi 3 Model B (RPi) and Intel® Core™ i7-4790K CPU @ 4.00GHz × 8 (desktop)

[![Car Detection with Intel NCS2 and Raspberry Pi](https://img.youtube.com/vi/HQSJFjbmng0/0.jpg)](https://www.youtube.com/watch?v=HQSJFjbmng0)

### Requirements
* Raspberry Pi 3 Model B
* Movidius Neural Compute Stick 2 (not tested yet on NCS)
* Webcam
* Display (Optional)

### Performance (RPi)

#### No Mask, without resizing
python3 realtime_objectdetection_and_tracking.py 
[INFO] starting video stream...
[INFO] frame size (W x H): 1920 x 1080


[INFO] elapsed time: 26.12
[INFO] approx. FPS: 46.51

#### Mask, resize
python3 realtime_objectdetection_and_tracking.py --mask 200,350,650,550 --resize 1024
[INFO] starting video stream...
[INFO] frame size (W x H): 1024 x 576
Observation mask (top left, bottom right): [(200, 350), (650, 550)]


[INFO] elapsed time: 28.05
[INFO] approx. FPS: 10.70

#### Mask

python3 realtime_objectdetection_and_tracking.py --mask 200,350,650,550
[INFO] starting video stream...
[INFO] frame size (W x H): 1920 x 1080
Observation mask (top left, bottom right): [(200, 350), (650, 550)]


[INFO] elapsed time: 21.76
[INFO] approx. FPS: 43.42

### Desktop

#### No mask, without resizing
python3 realtime_objectdetection_and_tracking.py 
[INFO] starting video stream...
[INFO] frame size (W x H): 1920 x 1080


[INFO] elapsed time: 23.19
[INFO] approx. FPS: 172.81

#### Mask
python3 realtime_objectdetection_and_tracking.py --mask 200,350,650,550
[INFO] starting video stream...
[INFO] frame size (W x H): 1920 x 1080
Observation mask (top left, bottom right): [(200, 350), (650, 550)]

[INFO] elapsed time: 20.83
[INFO] approx. FPS: 171.83



