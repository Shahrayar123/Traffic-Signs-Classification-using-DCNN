
# Traffic-Signs-Classification-using-CNN

In this project I used 
- Python
- Pickle
- Numpy
- Seaborn
- Matplotlib.pyplot
- Tensorflow

### **Clone dataset from [here](https://bitbucket.org/jadslim/german-traffic-signs/src/master/)**


The dataset contains 
- **34799** training images
- **4410** validation images
- **12630** testing images

Different traffic signs are available in dataset belonging to **43 classes**. In this project I made a model that predict a traffic sign with **95.15%** of testing accuracy.

<hr>

First I check the counts of images in train, validation and test dataset.

### **Counts of each class in dataset**

![train data counts](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/train_counts.png)


![validation data counts](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/val_counts.png)


![test data counts](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/test_counts.png)

<hr>

Then I display some random images with their labels from training, validation and test dataset

### **Training Images with labels**
![train data](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/train_data.png)

<br>

### **Validation Images with labels**
![validation data](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/val_data.png)

<br>

### **Test Images with labels**
![test data](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/test_data.png)

<hr>

After that I do some preprocessing, design CNN model architecture and compile model with 
- optimizer: `adam`  
- loss function : `categorical_crossentropy`
- metrics: `accuracy`

Then I write `callback` method to stop training of model when desired loss and accuracy will achieve
### After training the model the accuracy and loss is:


![accuracy and loss](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/acc_loss_visualization.png)

<br>

Then perform some prediction on unseen data and compare predicted result with acutal label

### **Model Prediction**
![accuracy and loss](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/predicted_images.png)

<br>

After that I plot confusion matrix to see the performance of model

### **Confusion Matrix**
![heatmap](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/heatmap.png)

Finally I test the model on new images and model give correct result

### **Prediction on Images**
![heatmap](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/stop_sign.png)

![heatmap](https://github.com/Shahrayar123/Traffic-Signs-Classification-using-CNN/blob/main/images/children_crossing_prediction.png)



