# DogRetrain
Machine learning project for retrain InceptionV3 using TensorFlow

Download Dataset from http://vision.stanford.edu/aditya86/ImageNetDogs/

## Setup

```console
conda create -n {env_name} python=3.6
conda env list
activate {env_name}
python -m pip install --upgrade pip
pip install tensorflow
pip install tensorflow-hub
cd {directory_path}\DogRetrain\code
```

## Retrain

```console
python retrain.py --image_dir {directory_path}\DogRetrain\dataset
```
## LABEL_IMAGE

```console
python label_image.py --graph=C:\tmp\output_graph.pb --labels=C:\tmp\output_labels.txt --input_layer=Placeholder --output_layer=final_result --image={directory_path}\DogRetrain\test\******.jpg
```
## TENSORBOARD

```console
tensorboard --logdir /tmp/retrain_logs
```
