# Batch-Normalization
This repo demonstrates the results of using 3 different Types of Normalization on the CIFAR dataset for a specific model architecture. The model architecture should be defined as ![image](https://github.com/iris-kurapaty/Batch-Normalization/assets/52544352/dfe841ec-3d5a-4846-8217-07a384c18dbe).

We can see the accuracy of the model built using < 50k parameters and running for a maximum of 20 epochs. The Jupyter Notebook contians all the 3 experiments with its logs. It uses modular code from model.py and utils.py from *src* folder to run different segments. The training and testing loss and accuracies for 20 epochs are available on the README file. 3 sets of misclassified images have been shared on the README file as well.

## Experiment Findings 
The best testing accuracy for the 3 methods are as follow:
1. Group Normalization: 71.54%
2. Layer Normalization: 59.79%
3. Batch Normalization: 74.77%

We see by keeping the model architecture similar, parameters < 50k and running for 20 epochs, that Batch Normalization performs the best among all 3 methods. In the logs its also noted that it reaches 70% accuracy the fastest among all 3. It also has the least amount of parameters. Layer Normalization performs the worst out of all, taking the most amount of parameters, we see a lot of more parameters assigned in the beginning few layers and lesser in the last layers which could amount the missclassificaiton rate. It's not the best suited method for the current problem. 

## Training and Testing Graphs

### Group Normalization
![image](https://github.com/iris-kurapaty/Batch-Normalization/assets/52544352/71183b39-951b-4a1f-a596-c22f2bc9a1d4)

### Layer Normalization
![image](https://github.com/iris-kurapaty/Batch-Normalization/assets/52544352/cf5c359b-7708-4a2d-9e6d-182ba93255ed)9

### Batch Normalization

![image](https://github.com/iris-kurapaty/Batch-Normalization/assets/52544352/3ccdbb7d-2c20-4677-9c4a-4ead7c3d5870)


## Misclassified Images

### Example 1
![image](https://github.com/iris-kurapaty/Batch-Normalization/assets/52544352/d4522945-5809-4fe8-a557-38c733194f06)

### Example 2
![image](https://github.com/iris-kurapaty/Batch-Normalization/assets/52544352/dc4e2f5a-f8d7-4a6a-9c34-c156f7b12ecd)

### Example 3
![image](https://github.com/iris-kurapaty/Batch-Normalization/assets/52544352/844128f8-2564-4c61-9a45-8f467a31c64e)


