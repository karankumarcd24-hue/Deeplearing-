# Object Detection Using EfficientDet and VGG16

## Program 1: Object Detection Using EfficientDet (One-Stage)

### Aim
To detect and identify objects in an image using a pre-trained EfficientDet model and display bounding boxes with class labels.

### Dataset Used
- **COCO Dataset (Common Objects in Context)**
- Contains 80 common object categories, such as people, cars, animals, and vehicles.
- A sample image is used for testing the pre-trained model.

### Results
The EfficientDet model detects multiple objects in the input image and displays labelled bounding boxes around them. It performs object detection in a single stage, making the process efficient.

---

## Program 2: Object Detection Using VGG16 and Selective Search (Two-Stage)

### Aim
To implement R-CNN-style object detection using Selective Search for region proposals and a pre-trained VGG16 model for object classification.

### Dataset Used
- **ImageNet Dataset**
- VGG16 is pre-trained on ImageNet, which contains 1,000 classification categories.
- A sample image is used to generate and classify candidate regions.

### Results
Selective Search generates possible object regions, and VGG16 classifies each region. High-confidence predictions are displayed with bounding boxes and labels. The two-stage approach requires more processing time because each proposed region is classified separately.

---

## Conclusion
Both programs demonstrate object detection using deep learning. EfficientDet performs detection in a single stage, while VGG16 with Selective Search uses a two-stage approach. EfficientDet is generally faster, whereas the VGG16 approach demonstrates region-based object detection.
