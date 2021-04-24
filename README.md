# Object-Detection
Real-time Object Detection using state-of-the-art You Only Look Once (YOLO) algorithm.


![ez2](https://user-images.githubusercontent.com/69038520/115949281-9fccba00-a4f1-11eb-98e9-ea2390e2f515.png)

## Requirements

1. [Tesorflow/Tensorflow-gpu](https://www.tensorflow.org/install/gpu) ([Compatibility](https://www.tensorflow.org/install/source#gpu))
2. [openCV](https://pypi.org/project/opencv-python/)
3. [Setting up Darkflow](https://github.com/thtrieu/darkflow)
4. [Weights and cfg file](https://pjreddie.com/darknet/yolo/)

 + Create a weights folder in darkflow and paste the weights in there.


### Processing a video using cmd.

 + Move the video into darkflow-master.
 + Open cmd from there and use the command.
 
 > python flow --model cfg/yolo.cfg --load weights/yolov2.weights --demo "video.mp4" --gpu 0.6 --saveVideo

 + Enter your video file name instead of "video.mp4"
 + Leave off --gpu 0.6 if you are not using Tensorflow-gpu.


### Swap out real-time detection to process a video.
   
  + Pass your file name as parameter instead of 0 in detection.py
```python
capture = cv2.VideoCapture("video.mp4")
```

 
