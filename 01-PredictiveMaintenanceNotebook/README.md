# Creating an R Notebook for Predicting Machine Failure

In this demo, we load data from a local file into R and explore it visually and statistically. Then, we will label anomalous data points to prepare data for modelling.

## Add data to a project

1. Download [sensorData](https://github.com/xnorax/watson-studio-journey/blob/master/data/sensorData.csv) file.

2. From your project's **Assets** page, click the **Find and add data** icon.

    ![1](https://github.com/xnorax/watson-studio-journey/blob/master/01-PredictiveMaintenanceNotebook/imgs/1.jpg?raw=true)


3. Click **Load** and then **browse** or drag sensorData.csv file onto the Load pane. You must stay on the page until the load is complete.

    ![2](https://github.com/xnorax/watson-studio-journey/blob/master/01-PredictiveMaintenanceNotebook/imgs/2.jpg?raw=true)

    The files now are saved in the object storage that is associated with your project and are listed as data assets on the Assets page of your project

    ![3](https://github.com/xnorax/watson-studio-journey/blob/master/01-PredictiveMaintenanceNotebook/imgs/3.jpg?raw=true)

## Create a Notebook
1. Click on **New notebook**.  
![4](https://github.com/xnorax/watson-studio-journey/blob/master/01-PredictiveMaintenanceNotebook/imgs/4.jpg?raw=true)

2. Select the **From URL** tab.

    ![5](https://github.com/xnorax/watson-studio-journey/blob/master/01-PredictiveMaintenanceNotebook/imgs/5.jpg?raw=true)

3. Configure your Notebook:
  1. Enter a name for your notebook in the **Name:** field.
  2. Paste [this URL](https://github.com/xnorax/watson-studio-journey/blob/master/01-PredictiveMaintenanceNotebook//PredictiveMaintenance.ipynb) in **Notebook URL** field.
  3. Choose R as a **runtime** environment.
  4. Click **Create Notebook**.

      ![6](https://github.com/xnorax/watson-studio-journey/blob/master/01-PredictiveMaintenanceNotebook/imgs/6.jpg?raw=true)

      Now you can see the notebook. It will have all the details for developing the model and deployment steps.  

      ![7](https://github.com/xnorax/watson-studio-journey/blob/master/01-PredictiveMaintenanceNotebook/imgs/7.jpg?raw=true)

      In the first cell, use **Insert to code** function to add automatically generated code to access the data.

      ![8](https://github.com/xnorax/watson-studio-journey/blob/master/01-PredictiveMaintenanceNotebook/imgs/8.jpg?raw=true)

      After running the notebook successfully, data will be ready to feed to Watson Machine Learning.
