#ML 

* Scaled automatically
* High-available, when configured to use multiple [[Availability Zone]]
### Features
#### Ground Truth
Set up and manage labeling jobs for training datasets using active learning and human labeling
#### Notebook
Access a managed Jupyter Notebook environment
#### Training
Train and tune models
#### Inference
Package and deploy your models
### Usage types
-|Offline Usage 💻|Online usage 🌐
--|--|--
Usage|Asynchronous or batch|Synchronous or real time
When|Generate predictions for an entire dataset all at once|Generate low-latency predictions
Method|SageMaker batch transform|SageMaker hsoting services
Input Format|Varies depending on algorithm|Varies depending on algorithm
Output Format|Varies depending on algorithm|JSON string

### Stages
#### Create a model
Provide predictions
#### Create an Endpoint Configuration
Specify the model to use, instance type, instance count, variant name and weight.
#### Create an Endpoint
The model is published and you can invoke it.

### Related
[[Amazon SageMaker Neo]]
[[Elastic Inference]]

### Source
https://learn.acloud.guru/course/certified-solutions-architect-associate/learn/31d7b2a1-17fa-44a4-87dc-a88315eec16e/c07ebb1b-6525-492c-907f-5299ec3bceed/watch