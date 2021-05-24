# Covid19 Detection from Chest-X-Ray

Coronavirus disease 2019 (COVID-19) is a highly infectious disease caused by severe acute respiratory syndrome coronavirus2 (SARS-CoV-2)

Currently Reverse transcription polymerase chain reaction (RT-PCR) is used for diagnosis of the COVID-19. 
X-ray machines are widely available and provide images for diagnosis quickly so chest X-ray images can be very useful in early diagnosis of COVID-19.

Large scale implementation of the COVID-19 tests which are extremely expensive cannot be afforded by many of the developing & underdeveloped countries hence if we can have some parallel testing procedures using Artificial Intelligence & Machine Learning, it will be extremely helpful.

Here, We have used **Transfer Learning** approach to build a Deep Learning based model to speed up the process of testing using chest x-ray. We have used the concept of explainable AI named as GradCAM to support our findings. 

> 1. Densnet
> 2. EfficientNetB7 
> 3. VGG16

We have used Chest X-ray (Covid-19 & Pneumonia) dataset from kaggle. 
Dataset contains Chest X-ray images of COVID-19, Pneumonia, & Normal patients.


## Transfer Learning

It is a method that allows us to use knowledge gained from other tasks in order tackle new but similar problems quickly and effectively.
It is used by loading a generic and well trained image classification network for feature extraction, and then adding few layers (head) to be trained for the target task.


## Data Description & Visualization

![download](https://user-images.githubusercontent.com/38699938/119252818-dc143880-bbcb-11eb-9f6b-294225c8e0af.png)

![download (1)](https://user-images.githubusercontent.com/38699938/119252823-e20a1980-bbcb-11eb-9cbf-525e096e0177.png)

![download (2)](https://user-images.githubusercontent.com/38699938/119252844-fbab6100-bbcb-11eb-837a-47c7955d0cac.png)

We can observe that images are of different sizes.


## Data preprocessing 

Images are scaled to a size of 244 by 244, Normalized to values (0,1) & augmented by simple zoom and rotation to enhance the generalization.

![download (3)](https://user-images.githubusercontent.com/38699938/119252908-4927ce00-bbcc-11eb-8694-d26efe7561e5.png)


## VGG16 loss and accuracy curves

![download-vgg](https://user-images.githubusercontent.com/38699938/119252798-b6872f00-bbcb-11eb-8b21-a73b5f121b42.png)


## Output of VGG16

![download (4)](https://user-images.githubusercontent.com/38699938/119252992-b20f4600-bbcc-11eb-9bb4-da4f43546a59.png)


