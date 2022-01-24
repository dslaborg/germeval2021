## GermEval 2021

Repository containing the experiments described in our paper for the [GermEval 2021 challenge](https://germeval2021toxic.github.io/SharedTask/): "Identifying German toxic, engaging, and fact-claiming comments with ensemble learning (FHAC at GermEval 2021)" ([available online](https://aclanthology.org/2021.germeval-1.16)).

The train and test data can be found in the folder [dataset](./dataset).
Experiments and their results are filed in [experiments](./experiments). 
The folder [figures](./figures) contains the scripts that were used to create the figures in our paper.

---
### Experiments

|number|description|single- or multi-label|
|---|---|---|
| |*model exploration*| |
|1|50 gelectra|multi-label|
|2|50 gbert|multi-label|
|3|25 gelectra + 25 gbert|multi-label|
|4|25 gelectra + 25 gbert|single-label|
| |*submissions*| |
|5|submission 1, 200 gelectra|multi-label|
|6|submission 2, 200 gelectra + 200 gbert|multi-label|
|7|submission 3, 30 gelectra + 30 gbert|single-label|

---
## Installation

The experiments were run in a conda environment with python 3.9.
You can find most of the required packages and the command for creating a new environemnt in the requirements.txt.
In addition to the packages described in the requirements.txt, two packages were installed using pip:
* `pip install emoji`
* `pip install transformers`
