# Fortnite Object Detection
Detection of player in fornite with AI (Yolo11)

#### Supported Labels
['head']

#### ALL my models YOLO11, YOLOv10 & YOLOv9
- Yolov9c: https://huggingface.co/jparedesDS/cs2-yolov9c
- Yolov10s: https://huggingface.co/jparedesDS/cs2-yolov10s
- Yolov10m: https://huggingface.co/jparedesDS/cs2-yolov10m
- Yolov10b: https://huggingface.co/jparedesDS/cs2-yolov10b
- Yolov10b: https://huggingface.co/jparedesDS/valorant-yolov10b
- Yolo11x: https://huggingface.co/jparedesDS/welding-defects-detection

#### How to use
```
from ultralytics import YOLO

# Load a pretrained YOLO model
model = YOLO(r'weights\fortnite-yolo11m.pt')

# Run inference on 'image.png' with arguments
model.predict(
    'image.png',
    save=True,
    device=0
    )
```
#### Confusion matrix normalized
![confusion_matrix_normalized.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/FafpmzBXEOs8JSYfbIEuk.png)
#### Labels
![labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/vOhmCFepNzzbWrlTwNyPC.jpeg)
#### Results
![results.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/scX2fjCVtt2qJHv8bL-zE.png)
#### Predict
![train_batch2.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/71tVmZsMl-G_aSG8-3czz.jpeg)
![train_batch1.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/ZoJbTl0LI5N8zncI0BstZ.jpeg)
```
YOLO11m summary (fused): 303 layers, 20,030,803 parameters, 0 gradients, 67.6 GFLOPs
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 1/1 [00:00<00:00, 41.69it/s]
                   all          1          7      0.987      0.857       0.87      0.832
```

#### Others models...
https://huggingface.co/jparedesDS/valorant-yolov10b
