# Learn how to use your own image inferencing model with Azure machine learning on edge



Follow the steps below

1. [Provision a Windows Data Science Virtual Machine (DSVM) on Azure](https://docs.microsoft.com/en-us/azure/machine-learning/data-science-virtual-machine/provision-vm) (Note that you can choose Linux as well if you are more comfortable with that).
2. Remote desktop into the DSVM using the admin account credentials that you configured when provisioning the DSVM.
3. Launch an "Anaconda Prompt" command window and type the command "activate AzureML". This will activate the AzureML environment. Run the following commands
  * pip install --upgrade azureml-sdk
  * pip install --upgrade onnxmltools
  * pip install git+https://github.com/apple/coremltools
  * md notebooks\AzureML\YoloV3
4. Copy onnx-deploy-yolov3.ipynb from this repo to notebooks\AzureML\YoloV3
5. Run the command "jupyter notebook". This will launch Jupter notebook server and open a browser window.
  * If you want to learn more about Jupyter notebook then go through an online tutorial, e.g. [Dataquest tutorial on Jupyter Notebook for Beginners](https://www.dataquest.io/blog/jupyter-notebook-tutorial/).
6. Navigate to /notebooks/AzureML/configuration.ipynb. Read through the notebook and follow the instructions. After going through this will have a configured Azure ML workspace.
7. Navigate to /notebooks/AzureML/YoloV3/onnx-deploy-yolov3.ipynb. This notebook will guide you through the process of deploying the YOLOv3 ONNX model as a webservice using Azure ML
