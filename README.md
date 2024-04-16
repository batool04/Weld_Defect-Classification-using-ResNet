# Weld_Defect-Classification-using-ResNet
The dataset is imported from Kaggle. The link of Kaggle dataset is "https://www.kaggle.com/code/sarahmacleans/detection-of-weld-defects". 
There are 6 different classes of weld defects and are given below:
good weld           0 , burn through        1 ,  contamination       2 ,  lack of fusion      3 , misalignment        4 , lack of penetration 5

### Good Weld (0):
This represents a weld that has been executed correctly, where the weld metal and base materials are appropriately fused without any visible defects, achieving structural integrity and the necessary aesthetic qualities.
### Burn Through (1):
This defect occurs when excessive heat causes the welding metal to melt through the workpiece, creating a hole or excessively thin section. It compromises the strength and appearance of the weld.
### Contamination (2): 
Contamination happens when foreign materials are introduced into the weld, such as dirt, oil, or rust. This can result in a weaker bond, visible impurities, and potentially lead to corrosion or failure of the weld.
### Lack of Fusion (3):
This defect is characterized by the failure of the weld metal to adequately fuse with the base metal or the preceding weld bead. It leads to weak joints that can easily break under stress.
### Misalignment (4): 
Misalignment, also known as poor fit-up, occurs when the parts to be joined are not properly aligned. This can lead to uneven stress distribution and a weak joint, affecting the overall functionality and strength of the assembly.
### Lack of Penetration (5):
This occurs when the weld does not penetrate fully into the joint, leaving part of the base material unfused. This creates a weak joint that may not withstand intended loads and can lead to failure under mechanical stress.

# Dataset Structure and Preprocessing
 ## Original Data Structure
The initial dataset was available in an unstructured format, where image files were scattered across various directories without a clear classification into the respective categories. There were no distinct folders corresponding to the six expected classes, which are essential for supervised learning tasks.

# Data Organization Process
To address this issue, we utilized an accompanying JSON file that contained mappings for each image to its corresponding class. This JSON file was crucial for categorizing the images into the six predefined classes: Good Weld, Burn Through, Contamination, Lack of Fusion, Misalignment, and Lack of Penetration.

# Steps Taken
 ### Reading JSON Mappings:
 We first loaded the JSON file to establish a connection between each image file and its designated class.
### Creating Class Directories:
Based on the JSON mappings, we programmatically created six separate folders, one for each class, to organize the images accordingly.
### Distributing Images:
Images were then moved to their respective class folders based on the information derived from the JSON file.
### Preparing Training and Testing Sets:
Once organized, the images were split into training and testing datasets. This split was essential for evaluating the performance of our model on unseen data.
