# Yolo_basketball_shot_predictor
## Ready-to-use Colab notebook: https://colab.research.google.com/drive/1Rksb3wYmM4jZXSsFAY84EDoJ97YgZ8V0?usp=sharing

https://user-images.githubusercontent.com/77502485/191056003-6fbaaeb2-bc2c-41ac-a64a-a02af07220b2.mp4


## Features
* The program draws a line between the ball and the rim and says if the line is valid or not for a point.
* Code can run on Both (CPU & GPU)

## Steps to run Code
* Download the pretrained model here: https://drive.google.com/file/d/1oTOnOOaFe5nVmgSXZw9PGOWltLyhIyb8/view?usp=sharing
```
!git clone https://github.com/WongKinYiu/yolov7
%cd yolov7
!pip install -r requirements.txt
%cd /content/yolov7
!wget "https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt"
```

### Using the shot predictor
* You have to upload the find_the_line.py in the directory of "yolov7" and for plots you have to upload find_the_line_plots in yolov7/utils 

```
!python find_the_line.py --weights /content/drive/MyDrive/Yolo_basketball_shooter/basketball.pt --conf 0.1 --source /content/drive/MyDrive/Basket_videos/vid3.mp4
```

