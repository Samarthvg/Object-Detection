# Object-Detection
Real-time Object Detection using state-of-the-art You Only Look Once (YOLO) algorithm.

### Requirements

1. [Tesorflow/Tensorflow-gpu](https://www.tensorflow.org/install/gpu)
2. [openCV](https://pypi.org/project/opencv-python/)
3. [Setting up Darkflow](https://github.com/thtrieu/darkflow)
4. [Getting the weights and cfg file](https://pjreddie.com/darknet/yolo/)

 + Create a weights folder in darkflow and paste the weights in there.

5. At this poit you can start proccessing a video.

 + Move the video into darkflow-master.
 + Open cmd from there and use the command.
 
 > python flow --model cfg/yolo.cfg --load weights/yolov2.weights --demo "video.mp4" --gpu 0.6 --saveVideo

 + Enter your video file name instead of "video.mp4"
 + Leave off --gpu 0.6 if you are not using Tensorflow-gpu.
 
