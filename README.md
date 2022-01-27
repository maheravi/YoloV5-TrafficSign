# Traffic Sign Detection Using YoloV5

![Alt text](https://github.com/maheravi/YoloV5-TrafficSign/blob/main/Sign.jpg "Optional title")

## Instalation

clone the repository:
```sh
$ git clone https://github.com/maheravi/YoloV5-TrafficSign.git

%cd YoloV5-TrafficSign

!pip install -U -r requirements.txt
```
## Dataset

The Dataser provided by Aryan Garg.
You can download it form the link below or downloading usinge the code in YoloV5_Traffic_Sign.ipynb

[Dataset link](https://drive.google.com/file/d/1gQD1OovQDyjMlUEWl6IEn2mzgS6KNppX/view)

## Train
```sh
!python train.py --img 640 --batch 16 --epochs 50 --data dataset.yaml --weights yolov5s.pt
```
## Test
```sh
!python val.py --data dataset.yaml --weights /content/yolov5/runs/train/exp/best.pt --img 640
```

## Inference
```sh
!python detect.py --source /content/yolov5/Sign.jpg --weights /content/yolov5/runs/train/exp/best.pt
```
