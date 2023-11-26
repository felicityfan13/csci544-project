# CSCI544-project
## Introduction
This repo contains file for model training for context-aware model using Tensorflow (support on CPU), and model training for fairseq model on GPU.
Data file (test) and build file are in cpu/scripts/data, cpu/scrpits/build
## Context-Aware model on CPU
### Run code
#### Create a conda environment
<img src="./conda.png" width="500">

#### bash train_baseline.sh -> this will create the basic translation model
<img src="./tokens.png" width="500">
change the REPO PATH to data to your local path

#### bash train_cadec.sh -> this will create the context-aware translation model
<img src="./checkpoint.png" width="500">
change the REPO PATH to data and model checkpoint to your local path

#### python test.py
The test accuracy is calculated on samples of different context ambiguity. Sample sentences:
<img src="./sample.png" width="500">

Test result is the accuracy of the translation of different phenomenon based on [data] (https://github.com/lena-voita/good-translation-wrong-in-context/tree/master/consistency_testsets)
<img src="./result.png" width="500">


## Reference repo:
##### 1. https://github.com/lena-voita/good-translation-wrong-in-context
##### 2. https://github.com/libeineu/Context-Aware
##### 3. https://github.com/neulab/contextual-mt
