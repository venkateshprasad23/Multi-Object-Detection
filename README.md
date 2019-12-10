# Multi-Object-Detection

Course Project for ECE 285 Special Topics in Robotics : Machine Learning for Image Processing

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

What things you need to install the software and how to install them

```
conda create -n Pullingos python=3.7 -y
conda activate Pullingos
conda install pytorch torchvision -c pytorch
git clone https://github.com/open-mmlab/mmdetection.git
cd mmdetection
python setup.py develop
```

### Installing

Follow the following commands to start training

```
git clone https://github.com/venkateshprasad23/Multi-Object-Detection
cd Multi-Object-Detection
python Training and Testing Codes/train.py Model Dictionaries/${CONFIG_FILE}
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```



