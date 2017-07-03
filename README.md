# A Low Latency Real-Time Object Detection App

## TLDR
This project uses a multithreaded approach to create a low latency real-time objection detection app. Built using Tensorflow's Object Detection API and OpenCV.

## Trying out the app
``` bash
git clone https://github.com/jamesloyys/Real-Time-Object-Detection.git
cd Real-Time-Object-Detection
python app_threaded.py
```
## Framework & Architecture
Many real-time object detection apps suffer from poor FPS (i.e. laggy video) due to the relatively slow performance of object detection models.

In order to achieve a smoother FPS, this project took a multithreaded approach (specifically, 2 threads) to separate the reading of frames from the webcam from the object detection model, achieving concurrency and parallelism.

This project also uses Tensorflow's newly released MobileNets family of lightweight computer vision models - perfect for the application that we're building here!

## Inspirations
This project was inspired by [Dat Tran's original work](https://medium.com/towards-data-science/building-a-real-time-object-recognition-app-with-tensorflow-and-opencv-b7a2b4ebdc32). I learnt alot from his post on Medium and wanted to improve on the FPS further. 



