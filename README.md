# Training YoloV3-Tiny on Google Colab

### Dataset Creation

Data collection and creation of a data set is first step towards training custom YoloV3 Tiny model. The best way to create data set is getting images and annotating them in the Yolo Format(*Not VOC*). According to me [labelImg](https://github.com/tzutalin/labelImg.git) is the best tool to annotate the dataset easily. It generates the .txt files containing the parameters of the bounding boxes in the image. Save these .txt files in the same folder as of the training images.

### Getting Files Ready

### Setting up Google Drive

The structure of your drive folder should be as follows:
```
.
└── yolo    
    ├── backup
    ├── obj
    │   ├── 1.jpeg
    │   ├── 1.txt
    │   ├── 2.jpeg
    │   ├── 2.txt
    │   ├── 3.jpeg
    │   ├── 3.txt
    │   └── other images and txt....
    ├── obj.data
    ├── obj.names
    ├── train.txt
    └── yolotiny.cfg
```
### Firing up the Colaboratory

Follow the [notebook](https://github.com/jayeshbhole/YoloV3-Tiny-Google-Colab/blob/master/Train_Tiny_YoloV3.ipynb) and get
your model training. After the training stops, the final weights will be saved in the backup folder of Google Drive.
