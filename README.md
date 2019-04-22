# yolov3_pytorch
基于pytorch的yolov3


# Training

** train your own datase

** --data-cfg='cfg/my.coco 

** change data/coco.names

** --coco=False

** Two style:** 1:coco style(class x y w h) xywh is Normalized

             ** 2:my dataset style(class x1 y1 x2 y2) xyxy is pixel
** if your dataset like coco style,please set --coco=True

** if set your own dataset,please set --coco=False

**Start Training:** Run `train.py` to begin training after downloading COCO data with `data/get_coco_dataset.sh`.


# Inference

Run `detect.py` to apply trained weights to an image, such as `zidane.jpg` from the `data/samples` folder:

**YOLOv3:** `detect.py --cfg cfg/yolov3.cfg --weights weights/yolov3.pt`
<img src="https://user-images.githubusercontent.com/26833433/50524393-b0adc200-0ad5-11e9-9335-4774a1e52374.jpg" width="700">

**YOLOv3-tiny:** `detect.py --cfg cfg/yolov3-tiny.cfg --weights weights/yolov3-tiny.pt`
<img src="https://user-images.githubusercontent.com/26833433/50374155-21427380-05ea-11e9-8d24-f1a4b2bac1ad.jpg" width="700">

## Webcam

Run `detect.py` with `webcam=True` to show a live webcam feed.

# Pretrained Weights

- Darknet `*.weights` format: https://pjreddie.com/media/files/yolov3.weights
- PyTorch `*.pt` format: https://drive.google.com/drive/folders/1uxgUBemJVw9wZsdpboYbzUN4bcRhsuAI

# 参考网址
- https://github.com/ultralytics/yolov3
- https://pjreddie.com/darknet/yolo/
- https://blog.csdn.net/leviopku/article/details/82660381
