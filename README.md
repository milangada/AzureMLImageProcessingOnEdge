# Learn how to use your own image inferencing model with Azure machine learning on edge

Specifically you will learn the following

1. Using an open source model (TinyYOLO) with Azure ML to convert the model to ONNX.
2. Package the model (along with the ONNX runtime) in a container with a scoring script.
3. Deploying the container on an Azure IoT Edge enabled device.
4. Use the REST endpoint on the container for image inferencing.

Follow the steps below

1. Provision a Windows Data Science Virtual Machine (DSVM) on Azure using instructions at https://docs.microsoft.com/en-us/azure/machine-learning/data-science-virtual-machine/provision-vm (Note that you can choose Linux as well if you are more comfortable with that).
2. Remote desktop into the DSVM using the admin account credentials that you configured when provisioning the DSVM.
3. Launch an "Anaconda Prompt" command window and type the command "activate AzureML". This will activate the AzureML environment. Run the following commands "pip install --upgrade azureml-sdk", "pip install --upgrade onnxmltools", and "pip install git+https://github.com/apple/coremltools". 
4. Double click on "Jupyter" shortcut that you see on the desktop. This will launch Jupyter notebook server and open a browser window. Go to Kernel menu and click on "Change kernel" to "Python [conda env:AzureML]". If you want to learn more about Jupyter notebook then go through an online tutorial (e.g. https://www.dataquest.io/blog/jupyter-notebook-tutorial/).
5. Browse to http://localhost:8888/notebooks/AzureML/configuration.ipynb. Read through the notebook and hit the "Run" button on the "Code" cells. Note that you will need to provide your Azure subscription id, Azure ML workspace name (if you already have one) along with the location. When generating the config file, you will be asked to login in to your Azure account. This will setup your Azure ML services workspace and configure your notebook library.
Browse to http://localhost:8888/notebooks/AzureML/how-to-use-azureml/deployment/onnx/onnx-convert-aml-deploy-tinyyolo.ipynb. This notebook goes over how to convert the TinyYOLO model from CoreML to ONNX and operationalize it as a web service using Azure Machine Learning services and the ONNX Runtime.
6. Go through the notebook documentation step by step. You can hit the "Run" button on the "Code" cells and see the results. 


