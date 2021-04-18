# Object-Detection
Real-time Object Detection using state-of-the-art You Only Look Once (YOLO) algorithm.


![prayerinc](https://user-images.githubusercontent.com/69038520/115148886-20696180-a07f-11eb-8caa-22af3df2025f.png)

## Requirements

1. [Tesorflow/Tensorflow-gpu](https://www.tensorflow.org/install/gpu)
2. [openCV](https://pypi.org/project/opencv-python/)
3. [Setting up Darkflow](https://github.com/thtrieu/darkflow)
4. [Weights and cfg file](https://pjreddie.com/darknet/yolo/)

 + Create a weights folder in darkflow and paste the weights in there.


### At this point you can start proccessing a video.

 + Move the video into darkflow-master.
 + Open cmd from there and use the command.
 
 > python flow --model cfg/yolo.cfg --load weights/yolov2.weights --demo "video.mp4" --gpu 0.6 --saveVideo

 + Enter your video file name instead of "video.mp4"
 + Leave off --gpu 0.6 if you are not using Tensorflow-gpu.


### Process video instead of real-time detection in code.
   
  + Pass your file name as parameter instead of 0. 
```python
capture = cv2.VideoCapture("video.mp4")
```

 
