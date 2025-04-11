# Counter Strike 2 Weapon Detector

#### Supported Labels
nc: 19
['AK47', 'M4A1-S', 'M4A1', 'GALIL', 'FAMAS', 'TEC-9', 'FIVE-SEVEN', 'GLOCK-18', 'USP-S', 'EAGLE', 'BERETTAS', 'P2000', 'MAC10', 'MP5', 'MP9', 'P90', 'P250', 'SSG08', 'AWP']

#### How to use
```
from ultralytics import YOLO

# Load a pretrained YOLO model
model = YOLO(r'weights\cs2-yolo12-weapon-detection.pt')

# Run inference on 'image.png' with arguments
model.predict(
    'image.png',
    save=True,
    device=0
    )
```

#### Labels
![labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/TRM3AEKgtpsc4Mq6MwyMx.jpeg)
#### Results
![results.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/toGWnn0SIJ_673BycYOes.png)
#### Predict
![val_batch1_labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/jP93wc2HietXSBScKUHOG.jpeg)
![train_batch2.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/NqxdnGl7_1H-Gr6TsOpWG.jpeg)
![train_batch0.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/S89frPmViNrtLjmEwD61y.jpeg)
```
YOLOv12m summary (fused): 169 layers, 20,119,561 parameters, 0 gradients, 67.2 GFLOPs
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 3/3 [00:01<00:00,  2.61it/s]
                   all         87        158      0.963          1      0.993      0.871
                  AK47         11         14      0.979          1      0.995      0.853
                M4A1-S          8         12      0.987          1      0.995      0.849
                  M4A1          9         13      0.978          1      0.995      0.844
                 GALIL          8         11      0.974          1      0.995      0.859
                 FAMAS          7          7      0.963          1      0.995      0.926
                 TEC-9          4          4      0.985          1      0.995      0.917
            FIVE-SEVEN          5          5       0.96          1      0.995      0.903
              GLOCK-18          4          4      0.932          1      0.995      0.905
                 USP-S         10         10      0.966          1      0.995        0.9
                 EAGLE          4          4      0.933          1      0.995      0.847
              BERETTAS          4          4      0.929          1      0.995      0.948
                 MAC10          6          6      0.953          1      0.995      0.891
                   MP5          7         11      0.978          1      0.995      0.852
                   MP9          7         11      0.978          1      0.995      0.888
                   P90          9         13      0.978          1      0.995      0.842
                  P250          6          6      0.977          1      0.995      0.861
                 SSG08          8         11        0.9          1       0.95      0.785
                   AWP          8         12       0.99          1      0.995      0.805
Speed: 0.2ms preprocess, 9.3ms inference, 0.0ms loss, 1.2ms postprocess per image
```

#### Others models Counter Strike 2 
https://huggingface.co/jparedesDS/
