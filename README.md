# RP-CNN
This is a PyTorch implementation of the paper "Random Part Localization Model for Fine Grained Image Classification". We present the test code on CUB-200-2011、Stanford Cars and FGVC-Aircrafts datasets for other researchers who interest in our work to reproduce our work.

## Requirements

The following are the experiment environment:
OS ubuntu 16.04
CUDA 9.0
CUDNN 7.0
Pytorch 0.4.1
4 NVIDIA 1080Ti GPU(at least 1 is required)
Note: please install jupyter to run the code provided.

## Datasets
You can download the three datasets from the official site:
for the bird dataset: 		http://www.vision.caltech.edu/visipedia/CUB-200-2011.html
for the car dataset:  		http://ai.stanford.edu/~jkrause/cars/car_dataset.html
for the aircraft dataset:	http://www.robots.ox.ac.uk/~vgg/data/fgvc-aircraft/
You should download the dataset and put it in the data folder. Then you should change the corresponding folder name in the code
(You must do it or the code can't find the image) to fit the train.txt/test.txt in the data folder.

Note: In the data folder, we provide the train/test list for all of the three dataset.

## Train the model
We provide the detailed codes to train the RP-CNN on all of the three dataset. You can just run the code we provided and you 
should get similar results.

## Test the model
If you want to test the code, you should first download the dataset, and then download the models, then you should put them in
the right folder, and you need to change the folder name in the code. Finally, Just run the jupyter notebook.

Note: There are some files named train_vectors_xx.npy, it is the object points localized using our proposed method. You can download it to test the model, or you can also generate it by yourself as we provide your the details in the file image_key_points_extraction.ipynb. 

## Model
We provide the trained model and associated files on https://pan.baidu.com/s/1cKVOBDFFi1dddF3eFPc_7Q. You can download them 
directly or you can choose to train from scratch.
