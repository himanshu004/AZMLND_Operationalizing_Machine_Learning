# Operationalizing Machine Learning

This project involves working with the [Bank Marketing Dataset](https://automlsamplenotebookdata.blob.core.windows.net/automl-sample-notebook-data/bankmarketing_train.csv). It includes model creation using Azure ML Studio, deploying it and then consuming the model through its API endpoints. Apart from that, it also includes creating a fully operational Machine Learning pipeline, publishing it as well as consuming it using Azure Python SDK.

## Architectural Diagram
The architecural diagram explains the flow of the project in a pictorial represenation. We start with installing the Azure az command line tool and create service principles(if we have our own subscription). We then create an Azure AutoML model using ML Studio and deploy the best model from the run. After enabling authentication, we enable Application Insights to maintain the logs of our model. We then use swagger to document model API structure, and thereafter consume the endpoints. We can also use Apache Benchmark tool for benchmarking the response, though it is not mandatory. Lastly, we publish a ML Pipeline using Azure Python SDK. 
<br></br> 
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/ArchDia.png)

## Key Steps
#### 1. Registering the dataset in Azure ML Studio.<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/dataset-avail.jpg)
<br></br>

#### 2. Creating the AutoML Model on the given dataset.<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/automl-model-creation.jpg)
<br></br>

#### 3. VotingEnsembleClassifier is the best model.<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/best-model.jpg)
<br></br>

#### 4. Enable Application Insights for logging.<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/aienabled.jpg)
<br></br>

#### 5. Run the logs.py script to observe the logs.<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/logsdotpy.jpg)
<br></br>

#### 6. Run the serve.py and swagger.sh files on localhost.<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/running-serve.py.jpg)
<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/running-swagger-container.jpg)
<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/swagger-localhost.jpg)
<br></br>

#### 7. Swagger running on localhost.<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/swagger1.jpg)
<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/swagger2.jpg)
<br></br>

#### 8. Run the endpoint.py script to get JSON output from the model.<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/endpoint.py.jpg)
<br></br>

#### 9. Pipeline is running in the Azure ML studio's pipeline section.<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/pipeline-running.jpg)
<br></br>

#### 10. Pipeline endpoint after publishing it.<br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/pipeline-endpoint.jpg)
<br></br>

#### 11. Bank Marketing Dataset with AutoML module. <br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/pipeline-automl.jpg)
<br></br>

#### 12. Published Pipeline overview showing REST endpoint and Active Status. <br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/activestatus.jpg)
<br></br>

#### 12. RunDetails Widget showing the step runs.  <br></br>
![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/jupyterrun.jpg)
<br></br>

![alt text](https://github.com/himanshu004/AZMLND_Operationalizing_Machine_Learning/blob/main/screenshots/scheduledrun1.jpg)
<br></br>


## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:

## Scope of improvement:
Providing the option of enabling deep learning during AutoML model creation would prove beneficial in terms of results and learning. Cross-comparing the models on factors like scoring metric, computational complexity, running time can also be added. 
More focus can be given on benchmarking content and different tools can also be compared.