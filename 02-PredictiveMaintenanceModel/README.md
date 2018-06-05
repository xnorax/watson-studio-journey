# Creating and Deploying a Predictive Maintenance Model

This tutorial will cover a full machine learning workflow starting from creating a model and ends up with testing a deployed mode.

# Steps
1. [Create a Model](##Step-1:-Create-a-Model)
2. [Add Your Data](##Step-2:-Add-Your-Data)
3. [Train Your Model](##Step-3:-Train-Your-Model)
4. [Evaluate Your Model](##Step-4:-Evaluate-Your-Model)
5. [Deploy Your Model](##Step-5:-Deploy-Your-Model)
6. [Test Your Model](##Step-6:-Test-Your-Model)


## Step 1: Create a Model
- From your project's **Assets** page, Click **New model**.

    ![1](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/1.PNG)

1. Enter a name for your model in the **Name:** field.
2. Associate the Model **Machine Learning Service** with the machine learning instance you created in [step 1](https://github.com/xnorax/watson-studio-journey/blob/master/###-Step-2:-Create-Machine-Learning-Instance) of setting up the project.
3. Select **Model builder** as a model type.
4. Select a **Spark Service** instance. If no instance is found, create one then click reload to select the newly created service.
5. Select **Automatic** model if you want to prepare your data and create a model automatically.

    *Manual option enable you to configure your own estimators in addition to some functions that are handled by the automatic data preparation.*
6. Click **Create**.

    ![2](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/2.PNG)


## Step 2: Add Your Data
1. Download [sensorTrainingData](https://github.com/xnorax/watson-studio-journey/blob/master/data/sensorTrainingData.csv) file.

2. From the action bar, click the **Find and add data** icon (![icon](![1](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/find_data_icon.png?raw=true))), and drag sensorTrainingData.csv file onto the Load pane.

3. On the **Select data asset** step, select *sensorTrainingData.csv* and click **Next**.  

    ![3](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/3.PNG)


## Step 3: Train Your Model
After successfully loading the dataset, you'll be redirected to the train step.
1. Select *target* in **Label Col** field.
2. Select all columns in **Feature columns** field.
    ![4](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/4.PNG)
3. After selecting a target and features of the dataset, the modeler will automatically suggest a technique, **Binary Classification** in our case, for building the model.
4. Optionally, adjust the validation split. By default this is set to Train: 60%, Test 20%, and Holdout: 20%.
5. After you are done making adjustments, click **Next**.

    ![6](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/6.PNG)

6. **Logistic Regression** algorithm will be selected automatically as an estimator.  
    ![8](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/8.PNG)

## Step 4: Evaluate Your Model
1. After the model is done training, the result of model evaluation will be presented under **performance**.

    ![9](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/9.PNG)

2. Click **Save** and **Save** again to confirm saving the model.

    You will be redirected to a summary about your model.  

      ![10](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/10.PNG)

## Step 5: Deploy Your Model
1. From the **Deployments** tab, click **Add Deployment**

    ![11](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/11.PNG)
<br></br>

2. On the **Create Deployment** page select a deployment type by clicking one of the following tabs:
- Web Service

  *that provides REST API to easily integrate with web and mobile apps*
- Batch Prediction

    *that predicts from sending batches of data at once*
- Real-time Streaming Predictions

    *that enable real-time prediction from data flows continuously*

    In this demo, we will deploy the model as a web service.

3. Type a name for your model in the **Name** field

4. Click **Save**.  
![12](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/12.PNG)

    Your deployed model should then appear in **Deployment** tab with *Deploy_Success* under **Status**.  
    ![13](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/13.PNG)

## Step 6: Test Your Model
1. Select the recent deployment.

    ![14](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/14.PNG)

2. From **Test** tab, enter some input data then hit **Predict**.  

    ![15](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/15.PNG)

3. View the prediction of target and the probabilities of the prediction.

    ![16](https://github.com/xnorax/watson-studio-journey/blob/master/02-PredictiveMaintenanceModel/images/16.PNG)
