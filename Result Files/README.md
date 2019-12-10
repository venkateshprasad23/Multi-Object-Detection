## Description

The test results have been written into Pickle files using ```test.py```, which are then read by another python program```voc_eval_fasterrcnn.py and voc_eval_cascadercnn.py``` to produce the results for our purpose 

```
xcascade.pkl             -- Result file of Cascade RCNN using ResNeXt50
results_resnet50.pkl     -- Result file of Faster RCNN using ResNet50
cascade.pkl              -- Result file of Cascade RCNN using ResNet50
xresnextfasterrcnn.pkl   -- Result file of Cascade RCNN using ResNeXt50
```

### Generating Result Pickle Files

Download the checkpoints from :\
```https://drive.google.com/drive/folders/15nKNvrvcy4eRfB0jK_awVdM5HEbaNjG7?usp=sharing```

Add them to your local clone of Multi-Object-Detection under a suitable directory. 

```
python Training and Testing Codes/test.py Model Dictionaries/FasterRCNN_ResNeXt50.py ${checkpoint file} --out results.pkl
```
