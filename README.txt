Chrysoprase Color Grading with Machine Learning

This repository contains the dataset and MATLAB scripts used in the study:

“Chrysoprase Color Grading with Machine Learning: A Systematic Approach.”

The repository also provides a standalone chrysoprase color classifier that can be used without installing MATLAB.

==================================================================================================

MATLAB RUNTIME (R2024a)

If you want to run the standalone chrysoprase color classifier (compiled application), MATLAB Runtime (R2024a) must be installed.

Verify that MATLAB Runtime (R2024a) is installed on your system.
If it is not installed, download it from the MathWorks website:

https://www.mathworks.com/products/compiler/mcr/index.html

Administrator privileges may be required to install MATLAB Runtime.

After installing MATLAB Runtime, the standalone classifier application can be launched directly.

==================================================================================================

REPRODUCING THE EXPERIMENTS

The machine learning experiments reported in the manuscript can be reproduced using the MATLAB scripts provided in this repository.

==================================================================================================

SOFTWARE ENVIRONMENT

MATLAB version
MATLAB R2024a

Required toolboxes

Statistics and Machine Learning Toolbox

Deep Learning Toolbox

==================================================================================================

DATASET

File
chrysoprase_color_dataset.xlsx

This file contains the colorimetric dataset used in this study.

Each row represents a color sample with the following variables:

Column 1 – L (CIELAB lightness)
Column 2 – a (CIELAB green–red coordinate)
Column 3 – b (CIELAB blue–yellow coordinate)
Column 4 – Label (color category assigned by clustering)

Note:
The chroma (C*) and hue angle (h°) reported in the manuscript are derived variables calculated from a* and b*.

==================================================================================================

REPRODUCIBILITY

To ensure reproducibility, a fixed random seed was used in all experiments:

rng(123,'twister')

The hyperparameters used in the models correspond to the final optimized values reported in the manuscript.

==================================================================================================

TRAINING SCRIPTS

The repository contains MATLAB scripts for training five machine learning models:

logistic.m – Logistic regression classifier
SVM.m – Support vector machine classifier
KNN.m – k-nearest neighbors classifier
randomforest.m – Random forest (bagged trees) classifier
neuralnetwork.m – Neural network classifier

Each script loads the dataset, trains the model, and outputs the classification results.

==================================================================================================

RUNNING THE CODE

Open MATLAB (R2024a)

Place all files in the same working directory

Run any of the following scripts:

logistic
SVM
KNN
randomforest
neuralnetwork

Each script will train the corresponding model and output the evaluation results.

==================================================================================================

CONTACT

If you have questions regarding the dataset, code, or classifier, please contact the corresponding author.