# Neural_Network_Charity_Analysis

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## **Project Overview**

Alphabet Soup, a philanthropic foundation dedicated to helping organisations that protect the environment, people’s well-being, and unify the world, has raised, and donated over ten billion dollars in the past 20 years. This money has been used to invest in life saving technologies and reforestation groups around the world. Beks, who oversees data collection and analysis for Alphabet Soup, has the job of analysing the impact of each donation and vet potential recipients to ensure the foundation’s money is being used effectively. To increase the likelihood of each donation being impactful, and in an effort to reduce fraud amongst recipients, Alphabet Soup’s president has asked Beks to determine which organisations are worth donating to and which are too high risk, by creating a mathematical, data-driven solution that can do this accurately. Beks has decided that due to the complexity of this task, she will design and train a deep learning neural network that will evaluate all types of input data and produce a clear decision-making result. This project will involve us helping Beks learn about neural networks and how to design and train these models using the Python TensorFlow library, that can be used to interpret large, complex datasets. 

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## **Resources**

-Data Source: charity_data.

-Software: Python 3.7.10; Visual Studio Code, 1.38.1; Jupyter Notebook; Anaconda3. 

-Resources: https://playground.tensorflow.org/; https://www.tensorflow.org; https://datascienceparichay.com/article/pandas-count-of-unique-values-in-each-column/; https://en.wikipedia.org/wiki/Hierarchical_Data_Format; https://machinelearningmastery.com/how-to-configure-the-number-of-layers-and-nodes-in-a-neural-network/.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## **Module 19 - Challenge** 

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Deliverable 1 – Preprocessing Data for a Neural Network Model 

A snapshot of the code used for Deliverable 1, can be found below. 

![Deliverable 1 - Image 1](https://user-images.githubusercontent.com/92111396/157316599-7971a9e1-99dd-4d4a-935a-5926ae9eefca.png)

![Deliverable 1 - Image 2](https://user-images.githubusercontent.com/92111396/157316611-334ee433-daf8-4f0b-9217-34ceff5ae75c.png)

![Deliverable 1 - Image 3](https://user-images.githubusercontent.com/92111396/157316616-bef637aa-ecc7-41a0-992c-24b4701eaad9.png)


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Deliverable 2 - Compile, Train, and Evaluate the Model

A snapshot of the code used for Deliverable 2, can be found below. 

![Deliverable 2 - Image 1](https://user-images.githubusercontent.com/92111396/157316952-31e71461-84e9-4758-8e9a-af2a5482d7f4.png)

![Deliverable 2 - Image 2](https://user-images.githubusercontent.com/92111396/157316971-efd23316-c759-4f1b-8dd9-2939ea4af622.png)


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Deliverable 3 - Optimize the Model

A snapshot of the code used for Deliverable 3, can be found below. 

![Deliverable 3 - Image 1](https://user-images.githubusercontent.com/92111396/157317622-b2735367-afb3-40fc-9495-bec0ff547ed5.png)

![Deliverable 3 - Image 2](https://user-images.githubusercontent.com/92111396/157317639-1bbc8173-327c-4e0c-8b0f-8b39478390e9.png)

![Deliverable 3 - Image 3](https://user-images.githubusercontent.com/92111396/157317655-ec0a3ba4-5795-43b9-a4de-fd797cacdf4f.png)

![Deliverable 3 - Image 4](https://user-images.githubusercontent.com/92111396/157317675-61da890b-8fd7-4459-9778-8d48f97a9343.png)

![Deliverable 3 - Image 5](https://user-images.githubusercontent.com/92111396/157317685-7d7b3e85-24c6-446f-b68a-445c854ed2b9.png)

![Deliverable 3 - Image 6](https://user-images.githubusercontent.com/92111396/157317695-98080b8e-71ca-4e28-8aa5-67ef24b1ff53.png)


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Deliverable 4 - A Written Report on the Neural Network Model

## **Purpose**

The purpose of this project is to help Beks create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup. From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. With our knowledge of machine learning and neural networks, we’ll use the features in the provided dataset to preprocess the data for a neural network model; compile, train and evaluate the model; and finally optimize the model, before producing a written report on the neural network model itself. 


The analysis focussed on answering the following questions divided into two categories:

Data Processing

1. What variable(s) are considered the target(s) for your model?
2. What variable(s) are considered to be the features for your model?
3. What variable(s) are neither targets nor features, and should be removed from the input data?

Compiling, Training, and Evaluating the Model

4. How many neurons, layers, and activation functions did you select for your neural network model, and why?
5. Were you able to achieve the target model performance?
6. What steps did you take to try and increase model performance?

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## **Results**

## **1. What variable(s) are considered the target(s) for your model?**

-The “IS_SUCCESSFUL” column is considered the target of the model.


## **2. What variable(s) are considered to be the features for your model?**

The below variables are considered to be the features of the optimized model:

-“APPLICATION_TYPE”

-“CLASSIFICATION” 

-“AFFILIATION” 

-“ORGANIZATION” 

-“STATUS”

-“INCOME_AMT”  

-“ASK_AMT”


## **3. What variable(s) are neither targets nor features, and should be removed from the input data?**

The below variables are neither targets nor features, and should be removed from the input data:

-"EIN"

-"NAME"

-"USE_CASE"

-"SPECIAL CONSIDERATIONS"


## **4. How many neurons, layers, and activation functions did you select for your neural network model, and why?**

I selected the following neurons, layers, and activation functions for my neural network.

**Attempt 1**
-2 Layers
-90 and 45 neurons
-Relu activation 
-40 epochs

**Attempt 2**
-3 Layers
-50, 30, and 10 neurons
-Relu activation 
-30 epochs

**Attempt 3**
-3 Layers
-80, 20, and 30 neurons
-Tanh activation 
-100 epochs

I selected each of these at random based on the trial-and-error method, in an effort to increase the predictive accuracy to 75%. At first, I simply increased the number of neurons to see if a simple solution, would lead to an increased level of predictive accuracy, but as was assumed, the problem was not simple enough to be linearly separated. As such, I made the decision to increase the layers, nodes, and epochs, in each subsequent attempt, to increase the level of accuracy, based on the principal of “going for depth” that states that “Empirically, greater depth does seem to result in better generalization for a wide variety of tasks”. 


## **5. Were you able to achieve the target model performance?**

-I was unable to achieve the target model performance of 75%.

-In retrospect or perhaps on a further attempt, I would have increased the level of layers to include more depth, as the increase in the amount of layers should allows the model to create more shapes and examples for classification to increase predictive accuracy. 


## **6. What steps did you take to try and increase model performance?**

I took the following steps to increase the model performance:

-Drop additional features (noisy variables) for all subsequent model configurations.

-Increase the layers 

-Increase/decrease the neurons in the additional layers

Each attempt can be explained as per the below.

**Attempt 1**
-2 Layers
-90 and 45 neurons
-Relu activation 
-40 epochs

**Attempt 2**
-3 Layers
-50, 30, and 10 neurons
-Relu activation 
-30 epochs

**Attempt 3**
-3 Layers
-80, 20, and 30 neurons
-Tanh activation 
-100 epochs

Below is a snapshot of the code used to increase model performance.

![Deliverable 3 - Image 1](https://user-images.githubusercontent.com/92111396/157323980-04f9864c-29d5-42e5-b08b-d7c899a62c07.png)

![Deliverable 3 - Image 2](https://user-images.githubusercontent.com/92111396/157323991-1691d3e9-28f8-4192-ad25-39e4c67be60f.png)

![Deliverable 3 - Image 3](https://user-images.githubusercontent.com/92111396/157324003-ac53a699-0db1-4bdf-9c98-2808b073462d.png)

![Deliverable 3 - Image 4](https://user-images.githubusercontent.com/92111396/157324014-5689fcda-2f8e-4428-a50e-6f2fb51578c5.png)

![Deliverable 3 - Image 5](https://user-images.githubusercontent.com/92111396/157324020-8769f5d0-3845-4db1-82a4-d9e6393454b5.png)

![Deliverable 3 - Image 6](https://user-images.githubusercontent.com/92111396/157324025-bcae3198-8600-48f9-86ba-4ff95cc88cd7.png)


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## **Summary**

Attempt 1:
Predictive Accuracy Percentage: 72%
Loss Metric: 56%

![Summary - Attempt 1](https://user-images.githubusercontent.com/92111396/157326733-a54d24c0-8c64-440e-ac87-772d20ed6d99.png)


Attempt 2:
Predictive Accuracy Percentage: 72%
Loss Metric: 55%

![Summary - Attempt 2](https://user-images.githubusercontent.com/92111396/157326768-b6af5239-eea2-4abd-9c08-f2c3e4d1b2b9.png)


Attempt 3:
Predictive Accuracy Percentage: 72%
Loss Metric: 57%

![Summary - Attempt 3](https://user-images.githubusercontent.com/92111396/157326797-25171191-77e1-4225-bc0a-3807d1f92e69.png)


**Recommendation**

While none of these models, achieved the predictive accuracy of 75%, for further attempts, I would recommend continuing to increase the level of hidden layers, so as to include more depth in the model to solve the classification problem. Increasing the depth (layers) of the model would allow for a greater creation of shapes and patterns of predictability; increasing the layers by a wide margin may create an upper bound, whereby I could then fine tune the model by varying the number of nodes, or by then decreasing the number of layers from the upper bound, based on a trial-and-error method.  

