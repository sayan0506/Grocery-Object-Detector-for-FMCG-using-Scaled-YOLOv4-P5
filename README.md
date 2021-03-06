# Build-and-Implement-ML-pipeline-an-Object-Detector-for-FMCG
Object Detector to detect the products present on the shelf for FMCG (Fast-Moving Consumer Goods)

# **Overview**

FMCG (Fast-Moving Consumer Goods) brands require insights into retail shelves to help them improve their sales. One such insight comes from determining how many products of their brands’ are present versus how many products of competing brands are present on a retail store shelf. This requires finding the total number of products present on every shelf in a retail store.


# **Problem Statement**

Object Detection problem statement [Deep Learning based Object Detector](https://drive.google.com/file/d/1yhqChbivg-N5C68uFkCJotf6y6Kr_ZsN/view)

# **Dataset**

* The dataset used for training/testing is the Grocery dataset. Link to the dataset: https://github.com/gulvarol/grocerydataset
* Please use the following link to download ShelfImages.tar.gz (contains train and test splits) and replace GroceryDataset_part1/ShelfImages with this https://storage.googleapis.com/open_source_datasets/ShelfImages.tar.gz

# **Approach**

We have used transfer learning for the object detection using scaled-Yolov4-P5. Considering compatibality and checking with image shapes, Yolov4-P5 is found suitable having image size 896. The model is pre-trained with Ms-coco dataset, was trained with the FMCG Grocery data for 110 epochs. The sample training performance can be found below:

![train](https://github.com/sayan0506/Grocery-Object-Detector-for-FMCG-using-Scaled-YOLOv4-P5/blob/main/images/results.png)

The sample inference of test data is given below:

![inference](https://github.com/sayan0506/Grocery-Object-Detector-for-FMCG-using-Scaled-YOLOv4-P5/blob/main/images/test_batch0_pred.jpg)

* *The detailed experiemnt result can be found from colab notebook [here](https://colab.research.google.com/drive/1Hb1ffz19UWf9kl_3EV9vktiQVvg5hEh4?usp=sharing).
* *All the documents regarding the experiment and model weights can be found from drive link [drive-yolov4](https://drive.google.com/drive/folders/1iN21WGeO0h-kKCTGcRpxFZwe71K3Zqdj?usp=sharing)

# **Reference**

* **[Mask RCNN on custom Dataset ](https://youtu.be/1u-dm5JMH1Q)**
* **[Simplifying Grocery Checkout with Deep Learning - CS230 ...](http://cs230.stanford.edu/projects_fall_2019/reports/26257432.pdf)**
* **[Detecting Objects in (almost) Real-time: FasterRCNN Explained with Code](https://towardsdatascience.com/fasterrcnn-explained-part-1-with-code-599c16568cff)**
* **[Faster R-CNN: Down the rabbit hole of modern object detection](https://tryolabs.com/blog/2018/01/18/faster-r-cnn-down-the-rabbit-hole-of-modern-object-detection/)**
* [Grocery-Product-Detection](https://github.com/sayakpaul/Grocery-Product-Detection)

**Object Detection Reference**

* [Evolution Of Object Detection Networks](https://www.youtube.com/playlist?list=PL1GQaVhO4f_jLxOokW7CS5kY_J1t1T17S)
* [YOLOv4 PyTorch](https://models.roboflow.com/object-detection/yolov4-pytorch)
* [Scaled YOLOv4 - Pytorch](https://models.roboflow.com/object-detection/scaled-yolov4)
* [YOLOv4-Large](https://github.com/WongKinYiu/ScaledYOLOv4)
* [Complete IoU(CIOU) Loss Intuitive Explanation](http://karthink.me/journal/Complete-IoU.html)
