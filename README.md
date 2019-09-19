# Detection-of-Pneumonia-from-Chest-X-Ray-Images Using 'InceptionV3 model' and 'CNN model'  

## Instructions:

To train "Inception v3" model for our own dataset follow the following instruction:

project file structure should be as following:

```
Transfer-Learning
| inception.model 
| README.md
| transfer.py
|__test_set
|   |__NORMAL
|   |    normal01.jpg
|   |    normal02.jpg
|   |    ...
|   |__PNEUMONIA
|   |    pneumonia01.jpg
|   |    pneumonia02.jpg
|   |    ..
|
|
|__training_set
|   |__NORMAL
|   |    normal01.jpg
|   |    normal02.jpg
|   |    ...
|   |__PNEUMONIA
|   |    pneumonia01.jpg
|   |    pneumonia02.jpg
|   |    ..
|
```

## Training Model

1. Download pretrained "InceptionV3" model using this [link](https://github.com/DhavalThkkar/Transfer-Learning/raw/master/inception.model)
2. Run python `transfer.py --nb_epoch 5 --batch_size 320 --plot --output_model_file filename.model`
3. Replace `filename` of above command with your own model name.
4. Later use the saved weights to predict any Image of cat or dog from the Internet or saved Images.

## Predicting the class

1. Open Jupyter Notebook file `predict_class.ipynb` and use `predict` function to predict class
2. In the `predict` function give image path and model name as `predict(img_path, model)`

## CNN Model

1. To use CNN model architecture run `Pneumonia_CNN.ipynb` jupyter notebook file. 
2. Set the number of epochs by trial and error method.
