# OpenCV-YOLOv3-Python-Pheasant-tailed Jacana

**Pheasant-tailed Jacana** detection with YOLOv3 on opencv-python.

You can change the detect object with your own training weights.

# Install requirements

```
$ pip install -r requirements.txt
```

# Detect images
First, download the pretrained weights from [here](https://drive.google.com/file/d/1ebXi5TXQh1OUu2_spayXL3VA25hQZTxq/view?usp=sharing) and put it to `yolo-bird`
directory.

Then type the following commands:
```
$ python yolo.py --image ./images/test.jpg --yolo yolo-bird
```

# Detect videos
If you follow the previous step to downloaded the pretrained weights, you could just type the following commands:
```
$ python yolo-video.py --input videos/test.mp4 --output output/test.avi --yolo yolo-bird
```
The result video will be saved in output/test.avi

# Take a Look at the yolo-bird folder:

**We will have 3 files inside**

1. **voc-bird.names :** The name of the object
2. **yolov3_10000.weights :** The weights we use as our detection model.
3. **yolov3-bird.cfg :** The configuration of our yolov3 model

# Reference

This project is based on the below articles:
- https://www.pyimagesearch.com/2018/11/12/yolo-object-detection-with-opencv/
- https://cuda-chen.github.io/programming/2019/11/29/a-detailed-guide-of-yolo-on-opencv-python.html
