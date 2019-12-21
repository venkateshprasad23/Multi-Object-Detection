# Multi-Object-Detection

Course Project for ECE 285 Special Topics in Robotics : Machine Learning for Image Processing, completed by Team Pullingos.

## Description

Please refer to ```MOD_Report.pdf``` for a detailed report in the NIPS Conference Template.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Run the following commands to set up your environment for the project.

```
conda create -n Pullingos python=3.7 -y
conda activate Pullingos
conda install pytorch torchvision -c pytorch
git clone https://github.com/venkateshprasad23/Multi-Object-Detection
python setup.py develop
```
### Code Organisation

Code organisation has been done individually for each folder.

### Training

Execute the following commands to start training.
```
python Training and Testing Codes/train.py Model Dictionaries/${CONFIG_FILE}
```
Choose a config file of your choice from the Model Dictionaries directory.

If your training suspends mid-way, and you need to resume from the latest checkpoint, use the command below.

```
python Training and Testing Codes/train.py Model Dictionaries/${CONFIG_FILE} --resume_from=${checkpoint file}
```

### Testing

If you need to test your model and print its Mean Average Precision, you have to pass the pickle file as an argument\
to ```voc_eval_cascadercnn.py``` or ```voc_eval_fasterrcnn.py```.

```
python Training and Testing Codes/voc_eval_fasterrcnn.py ${Result File} ${Model Config File}
```

### Running demo

The demo has been developed on Google Colab. The Jupyter Notebook file of the same has been uploaded here.

Here's a link to the same : ```https://colab.research.google.com/drive/1ZGeOyMdLHNV82gRZC2Qad5jHTFE2VSxH```

If you plan to run the demo in Colab, please download the checkpoint file, config file and the demo image
from this link : ```https://drive.google.com/drive/folders/16_E6UkY00AOnBQm4eSqSuUatWL7Ls6el?usp=sharing```

Upload them to your Google Drive and update the directory pointing to the these three variables in the Colan Notebook. After that, just run the rest of the cells as it is. It wil install all the required packages for you.

If you plan to run it on UCSD DSMLP cluster, then, use the ```demo.ipynb``` file uploaded here. Change the directory to the three variables in the file after uploading them to DSMLP. After that, just run the rest of the cells as it is. It will install all the required packages for you.

### Team Members
Venkatesh Prasad Venkataramanan\
Shakeel Ahamed Mansoor Shaikna\
Siddarth Meenakshi Sundaram\
Zirui Wang.


