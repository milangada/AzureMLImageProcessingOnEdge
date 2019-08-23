# Learn how to use your own image inferencing model with Azure machine learning on edge



Follow the steps below

1. [Configure your development environment](https://docs.microsoft.com/en-us/azure/machine-learning/service/how-to-configure-environment#local). Make sure you follow all the instructions and install Jupyter Notebooks as well.
2. [Install Docker](https://docs.docker.com/docker-for-windows/install/). Docker on your machine will enable you to deploy and test the service locally before deploying it to the cloud. Note that Docker for Windows supports running Linux images on Windows 10 (but not on Windows server)
4. Copy onnx-deploy-yolov3.ipynb and yolov3_classes.txt from this repo to notebooks\AzureML\YoloV3
5. Run the command "jupyter notebook". This will launch Jupter notebook server and open a browser window.
  * If you want to learn more about Jupyter notebook then go through an online tutorial, e.g. [Dataquest tutorial on Jupyter Notebook for Beginners](https://www.dataquest.io/blog/jupyter-notebook-tutorial/).
6. Navigate to /notebooks/AzureML/configuration.ipynb. Read through the notebook and follow the instructions. After going through this will have a configured Azure ML workspace.
7. Navigate to /notebooks/AzureML/YoloV3/onnx-deploy-yolov3.ipynb. This notebook will guide you through the process of deploying the YOLOv3 ONNX model as a webservice using Azure ML

1. [Provision a Windows Data Science Virtual Machine (DSVM) on Azure](https://docs.microsoft.com/en-us/azure/machine-learning/data-science-virtual-machine/provision-vm) (Note that you can choose Linux as well if you are more comfortable with that).
2. Remote desktop into the DSVM using the admin account credentials that you configured when provisioning the DSVM.
3. Using PowerShell command window run the following commands to update docker to the latest version. 
 * Install-Package -Name Docker -ProviderName DockerMSFTProvider -Update -Force
 * Restart-service docker
Launch an "Anaconda Prompt" command window and type the command "activate AzureML". This will activate the AzureML environment. Run the following commands
  * pip install --upgrade azureml-sdk
  * md notebooks\AzureML\YoloV3
4. Copy onnx-deploy-yolov3.ipynb and yolov3_classes.txt from this repo to notebooks\AzureML\YoloV3
5. Run the command "jupyter notebook". This will launch Jupter notebook server and open a browser window.
  * If you want to learn more about Jupyter notebook then go through an online tutorial, e.g. [Dataquest tutorial on Jupyter Notebook for Beginners](https://www.dataquest.io/blog/jupyter-notebook-tutorial/).
6. Navigate to /notebooks/AzureML/configuration.ipynb. Read through the notebook and follow the instructions. After going through this will have a configured Azure ML workspace.
7. Navigate to /notebooks/AzureML/YoloV3/onnx-deploy-yolov3.ipynb. This notebook will guide you through the process of deploying the YOLOv3 ONNX model as a webservice using Azure ML
