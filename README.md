# Fortnite Object Detection
Detection of player in fornite with AI (Yolo11)

#### Supported Labels
['head', 'player']

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
![confusion_matrix_normalized.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/B9zPmKLks9x92bQ71W4WN.png)
#### Labels
![labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/CSgOxmA86zJ8Bav6ChqOK.jpeg)
#### Results
![results.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/3oSidFJgQyJL0JZS0nbZW.png)
#### Predict
![val_batch1_pred.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/PxU0FT1r34-cg98lLJUiw.jpeg)
![val_batch2_labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/Ltah8kdNiv6GE1knl0HWv.jpeg)
![val_batch2_pred.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/A84rA88ASXon1QL96xhOG.jpeg)
```
YOLO11m summary (fused): 303 layers, 20,031,574 parameters, 0 gradients, 67.7 GFLOPs
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 12/12 [00:06<00:00,  1.90it/s]
                   all       1014       2097      0.933      0.739      0.828      0.668
                  head        223        633      0.947      0.738      0.825      0.664
                player        990       1464      0.919       0.74      0.831      0.673
````

#### Others models...
https://huggingface.co/jparedesDS/valorant-yolov10b
