<h1> Object detection using yolov8 </h1>
<p>Trained a YoloV8 model to detect two classes - Pen, Glasses </p1>

<p align="center">
  <img src="/imgs/pen.jpg" width="200" hspace="20"/>
  <img src="imgs/glasses.jpg" width="200" hspace="20"/> 
</p>

<p>Training data and was used from Google open images</p>
  <img src="https://cdn.analyticsvidhya.com/wp-content/uploads/2018/05/Open-Images.png" width="400" hspace="300"/> 
<br>
<br>
<p> You can load the trained weights and predict on new data by code below </p>

```python
model = YOLO("/runs/detect/train3/weights/best.pt")
results = model.predict("/path-to-data", save=True, imgsz=320)
```


<h2>My Training results</h2>
<h4>Training </h4>
<p align="center">
  <img src="/runs/detect/train3/train_batch1.jpg" width="400" hspace="20"/>
  <img src="/runs/detect/train3/train_batch2.jpg" width="400" hspace="20"/>
</p>

<h4>Validation</h4>
<p align="center">
  <img src="/runs/detect/train3/val_batch0_labels.jpg" width="400" hspace="20"/>
  <img src="/runs/detect/train3/val_batch0_pred.jpg" width="400" hspace="20"/>
</p>
<br>
<br>
<h2>Inference on new data</h2>
<p align="center">
  <img src="/runs/inference-6.png" width="400" hspace="20"/>
  <img src="/runs/inference-2.png" width="400" hspace="20"/>
</p>

<p align="center">
  <img src="/runs/inf3.gif" width="600" height="400" />
</p>
