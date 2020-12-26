# Operationalizing Machine Learning

This project involves working with the [Bank Marketing Dataset](https://automlsamplenotebookdata.blob.core.windows.net/automl-sample-notebook-data/bankmarketing_train.csv). It includes model creation using Azure ML Studio, deploying it and then consuming the model through its API endpoints. Apart from that, it also includes creating a fully operational Machine Learning pipeline, publishing it as well as consuming it using Azure Python SDK.

## Architectural Diagram
The architecural diagram explains the flow of the project in a pictorial represenation. We start with installing the Azure az command line tool and create service principles(if we have our own subscription). We then create an Azure AutoML model using ML Studio and deploy the best model from the run. After enabling authentication, we enable Application Insights to maintain the logs of our model. We then use swagger to document model API structure, and thereafter consume the endpoints. We can also use Apache Benchmark tool for benchmarking the response, though it is not mandatory. Lastly, we publish a ML Pipeline using Azure Python SDK. 
<br> 
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/ArchDia.png)

## Key Steps
1. Registering the dataset in Azure ML Studio.
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/dataset-avail.jpg)


## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:
