# Learn how to use your own image inferencing model with Azure machine learning on edge



Follow the steps below


1. [Install Docker](https://docs.docker.com/docker-for-windows/install/). Docker on your machine will enable you to deploy and test the service locally before deploying it to the cloud. Note that Docker for Windows supports running Linux images on Windows 10 (but not on Windows server)
2. [Configure your development environment](https://docs.microsoft.com/en-us/azure/machine-learning/service/how-to-configure-environment#local). Make sure you follow all the instructions and install Jupyter Notebooks as well.
3. Create a folder called YoloV3 under notebooks\AzureML and copy onnx-deploy-yolov3.ipynb, yolov3_classes.txt, and iotedge-yolov3-template from this repo to that folder
4. Run the command "jupyter notebook". This will launch Jupter notebook server and open a browser window. If you want to learn more about Jupyter notebook then go through an online tutorial, e.g. [Dataquest tutorial on Jupyter Notebook for Beginners](https://www.dataquest.io/blog/jupyter-notebook-tutorial/).
5. Navigate to /notebooks/AzureML/configuration.ipynb. Read through the notebook and follow the instructions. After going through this will have a configured Azure ML workspace.
6. Navigate to /notebooks/AzureML/YoloV3/onnx-deploy-yolov3.ipynb. This notebook will guide you through the process of deploying the YOLOv3 ONNX model as a webservice using Azure ML.
