### Various YOLO versions for trash detection.
YOLO/Dataset | Trash<br>Flowrate |  |  | FloW |  |  | Trash<br>ICRA |  |  |
--- | --- | --- | --- |--- |--- |--- |--- |--- |--- |
--- | mAP<br>@50 | mAP<br>@75 | mAP<br>@50:95 |mAP<br>@50 | mAP<br>@75 | mAP<br>@50:95 |mAP<br>@50 | mAP<br>@75 | mAP<br>@50:95 |
YOLOv5n | 90.1 | 53.4 | 51.6 | 83.0 | 34.6 | 40.6 | 96.4 | 80.5 | 68.9 |
YOLOv5l | 92.8 | 59.4 | 55.9 | 87.0 | 36.1 | 43.4 | 97.6 | 88.8 | 76.1 |
YOLOv6n | 84.3 | 35.8 | 42.3 | 84.3 | 35.8 | 42.3 | 96.3 | 84.6 | 74.7 |
YOLOv6l | 91.7 | 57.8 | 55.1 | 87.8 | 37.6 | 44.6 | 97.3 | 88.4 | 77.1 |
YOLOv7t | TBA | TBA | TBA | TBA | TBA | TBA | 90.1 | 72.7 | 59.9 |
YOLOv7 | TBA | TBA | TBA | TBA | TBA | TBA | 94.2 | 80.0 | 68.5 |
YOLOv9 (GELAN-C) | **`94.0`** | **`66.1`** | **`60.7`** | 88.6 | 41.7 | **`46.2`** | **`98.7`** | **`93.1`** | **`83.5`** | 
Transformers | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD |

### State-of-the-art results:

Dataset | Method | mAP@50 | mAP@50:95 | Condition
--- | --- | --- | --- | --- |
Trash<br>Flowrate<sup>1</sup> | M2DET | - | 45.8 | Above<br>water | 
FloW<sup>2</sup> | YOLOv7-ACELAN | 44.0 | **`90.3`** | Above<br>water
TrashICRA<sup>3</sup> | Faster-RCNN | 96.7 | 74.1 | Under<br>water

<sup>1</sup>https://www.researchgate.net/publication/356793137_Trash_Detection_on_Water_Channels

<sup>2</sup>https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4758755

<sup>3</sup>https://ieeexplore.ieee.org/abstract/document/10249233

### Trash-ICRA Confusion Matrix and Precision-Recall Curve:
<p align="center">
  <img src='https://github.com/ongacoder1/yolo_trash/blob/main/images/cm_trashicra.png' width=30%, height=30%>
  <img src='https://github.com/ongacoder1/yolo_trash/blob/main/images/pr_trashicra.png' width=40%, height=40%>
</p>

### Trash-ICRA Metrics:

Class     | Images | Instances | P     | R  | mAP@50 | mAP@50:95 |
---       | ---    | ---       | ---   |--- |---     |---        |
all       | 1144   | 1668      |96.8       |97.0      |98.7      |83.5|
plastic   | 1144   |  937      |99.1      |98.5      |99.4      |78.5|
bio       | 1144   |  396      |97.4      |96.7      |99.0       |85.0|
rov       | 1144   |  335      |93.9      |95.8      |97.5      |86.9|
