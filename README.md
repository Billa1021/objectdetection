# objectdetection

annotations: This folder will be used to store all respective TensorFlow *.record files, which contain the list of annotations for our dataset images.

exported-models: This folder will be used to store exported versions of our trained model(s).

images: This folder contains a copy of all the images in our dataset, as well as the respective *.xml files produced for each one, once labelImg is used to annotate objects.

images/train: This folder contains a copy of all images, and the respective *.xml files, which will be used to train our model.

images/test: This folder contains a copy of all images, and the respective *.xml files, which will be used to test our model.

models: This folder will contain a sub-folder for each of training job. Each subfolder will contain the training pipeline configuration file *.config, as well as all files generated during the training and evaluation of our model.

pre-trained-models: This folder will contain the downloaded pre-trained models, which shall be used as a starting checkpoint for our training jobs.

Preparing the Dataset:-

We installed labelimg by using pip install labelimg.which used to label the objects in the Training data.TensorFlow requires a label map, which namely maps each of the used labels to an integer values. This label map is used both by the training and detection processes. Label map files have the extention .pbtxt

 We have to convert our annotations into the so called TFRecord format.
 
Model selection:-
The SSD ResNet50 V1 FPN 640x640 model, since it provides a relatively good trade-off between performance and speed. However, there exist a number of other models we can use, all of which are listed in TensorFlow 2 Detection Model Zoo

I trained my model and the objects got detected from test folder.
