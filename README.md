# bi-class_Semantic_Segmentation
A modification of Semantic Segmentation package (https://github.com/GeorgeSeif/Semantic-Segmentation-Suite) for bi-class segmentation of images)
This package is a modification of George Seif semantic segmentation package (https://github.com/GeorgeSeif/Semantic-Segmentation-Suite)

The current package is different from the original one is the following ways: 

1- The current package is customized for bi-class segmentation with an example on images of a cracked area (two classes: crack and background). 

2- The current package is customized is customized to handle images with significant class imbalnace in the pixels 

3- A new model (FC_Dense_NetAA) is added in FC_DenseNet_Tiramisu.py code in the models folder. The newly introduced model has a simpler structure
in comparison to the original 100 layer Tiramisu and is specifically fabricated for the relatively simple case of bi-class semantic segmentation

4- Grid search files (with "_GS_AA" suffix in their name) are added to do a grid search regarding the newly introduced model (FC_DenseNetAA) or any other model

5- In the case of grid search, the user has to determine the search intervals (discrete values) corresponding to each of the hyperparameters of the interest

6- In the case of grid search, chechpoints corresponding to each of the explored models are saved in the checkpoints folder.

7- Pixelcounter.py is a code for counting crack pixels and estimation of crack length in the specific case of segmented images of a cracked area.


To use this modified package, the user may start with ReadME file of the original package (https://github.com/GeorgeSeif/Semantic-Segmentation-Suite) and then continue with this ReadME file.
