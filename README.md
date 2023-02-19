## Transportation_Vehicle_Type_Classification

# Introduction
Transportation is one of the most essential life aspects. Machine learning has added a lot through classification, detection and segmentation. This project deals with images of different types of transportation vehicles as its data and classify the input picture which can be useful in many industries.

# Problem statement
Vehicles’ types classification is essential nowadays in many forms. It aims to identify which vehicle is being seen by a machine. It can be used in many applications such as surveillance, cars’ detection systems, traffic systems and more.

# Datasets
The collected images dataset consists of 10 classes, (Airplane, Car, Bus, Boat, Bike, Motorcycle, Scoter, toktok, Tram and Truck). Every class consists of 50 images.
The data has been split into 80% training (20% for validation), and 20% for testing. All the images were resized to 64*64 pixels.

# Methods
Three different models were used:
Firstly, a sequential CNN model is used to classify the images with relu activation function and softmax in the output layer.
VGG16 model was used by freezing all the weights of the network and adding new layers.
The third model is VGG16 model with leaving the last 2 layers unfreeze for fine-tuning.
![image](https://user-images.githubusercontent.com/47840840/219969498-d75bd454-94cc-42f6-b11e-af778e648ced.png)

# Evaluation

![image](https://user-images.githubusercontent.com/47840840/219969526-291eb8ad-94da-4917-acb3-ad37ef201595.png)
![image](https://user-images.githubusercontent.com/47840840/219969527-ccfb7089-3d88-4950-873f-62f64c4ef454.png)
![image](https://user-images.githubusercontent.com/47840840/219969532-8ded3ae7-092f-4de0-aaef-cdb5d1bd793d.png)
![image](https://user-images.githubusercontent.com/47840840/219969540-1884dd98-30de-4296-8d4a-20abc8fa21fb.png)


# Conclusion
Ensemble method was used which calculates the mode between different models that surely have different errors, the output is more robust.
The difference between validation loss and training loss decreases when applying regularization.
After applying data augmentation, the accuracy increased as the applied data samples increased.
The training and validation accuracies increased slightly after using data augmentation with regularization in both VGG16 models.


