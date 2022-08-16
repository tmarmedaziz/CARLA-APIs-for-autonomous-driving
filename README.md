<h1 align="center">zd CARLA-APIs-for-autonomous-driving</h1>
<h3 align="center">My first steps into ADAS and smart vehicles world</h3>



## Context

This project was carried out as part of the career preparation project, the result of hard work and dedication, and is supervised by Ms. Ferdaous Chaaben. It is a simple discovery of the automotive world and ADAS systems.

## Pipeline

The project was divided into three parts (object detection, Drivable area detection and integration of models in CARLA). So, after training and getting good results for the models, we can extract from a street image the elements around the vehicle and the drivable area.
Then, while working on the CARLA (CAR Learning to Act) simulator, I generate APIs to get results on the simulator.

## Dataset
I worked on BDD100k dataset [Berkley dataset](https://drive.google.com/file/d/17QDoDyQcH1cFSHfoBprNWz9i-_nEQm4K/view?usp=sharing) which this drive link is the compressed data you will use for each model training

## Drivable area detection
I am working on a subset of the dataset. I trained the U-Net model several times with different sizes and input parameters for binary semantic segmentation to extract the street. With some filters and traditional computer vision methods, I was able to extract the green lane where to drive safely. You find the trained weights in [this link](https://drive.google.com/file/d/1t6pNvmg9ZqLfIbj6AzHYb0CcbzGfS0ao/view?usp=sharing)            
Here is an example of the result (lines are well-marked):
![alt text](https://i.postimg.cc/pXz8LdWL/lane-result.jpg)

## Object detection
For object detection, I trained YoLov4 on a custom dataset in google colab to get better results.
I worked on the official darknet framework, then extracted the trained weights to do the inference. You find the trained weights in [this link](https://drive.google.com/drive/folders/1Hfg9HSOBppiRLDPRZ-4TsmyF6DgP7-Ru?usp=sharing)   
Here is an example of the result:
![alt text](https://i.postimg.cc/d0PTPcPT/od.jpg)

## Simulator
At the end of this project, I generated an API to run these models on CARLA.
![alt text](https://i.postimg.cc/x8xHh9mV/full.jpg)

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://opencv.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg" alt="opencv" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://seaborn.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://seaborn.pydata.org/_images/logo-mark-lightbg.svg" alt="seaborn" width="40" height="40"/> </a> <a href="https://www.tensorflow.org" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg" alt="tensorflow" width="40" height="40"/> </a> </p>


## License
[Tmar Mohamed Aziz](https://www.linkedin.com/in/tmar-med-aziz/)
