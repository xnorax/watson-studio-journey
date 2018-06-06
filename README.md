# IBM Watson Studio Journey

This repository demonstrates different capabilities of IBM Watson Studio.

> It provides a suite of tools for data scientists, application developers and subject matter experts to collaboratively and easily work with data and use that data to build, train and deploy models at scale.

## Guide
We will start the journey by importing a notebook for labelling anomalous data to prepare data for modelling [[1]](https://github.com/xnorax/watson-studio-journey/tree/master/01-PredictiveMaintenanceNotebook). Then, we will do a complete machine learning process starting from creating a model and ending with testing a deployed model [[2]](https://github.com/xnorax/watson-studio-journey/tree/master/02-PredictiveMaintenanceModel). In the third tutorial, we will build a flow to compare between multiple models [[3]](https://github.com/xnorax/watson-studio-journey/tree/master/03-PredictiveMaintenanceFlow). Next, we will build an image classifier for pipeline inspection [[4]](https://github.com/xnorax/watson-studio-journey/tree/master/04-PipelineVisualRecognition). Finally, we will create and share an interactive dashboard which helps to discover insights from your data [[4]]([[3]](https://github.com/xnorax/watson-studio-journey/tree/master/05-AnalyticsDashboard)).

## Prerequisites
- [IBM Cloud Account](https://ibm.biz/BdZzCd)

  **Note**: Select *United States/US-South* as a country.

- An IBM Cloud Object Storage instance
- An IBM Watson Machine Learning instance

## Steps
- [Step 1: Create Object Storage Instance](#step-1-create-object-storage-instance)
- [Step 2: Create Machine Learning Instance](#step-2-create-machine-learning-instance)
- [Step 3: Create Watson Studio Instance](#step-3-create-watson-studio-instance)
- [Let's Get Started](#lets-get-started)

### Step 1: Create Object Storage Instance
- from the IBM Cloud catalog, select **Object Storage**.  

  ![1](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/1.jpg?raw=true)
- Click **Create**.

  ![2](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/2.jpg?raw=true)  

  You'll be redirected to your service instance dashboard.  
  ![3](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/3.jpg?raw=true)  
<br></br>

### Step 2: Create Machine Learning Instance
- from Watson category in the IBM Cloud catalog, select **Machine Learning**.

  ![4](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/4.jpg?raw=true)

- Click **Create**.  

  ![5](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/5.jpg?raw=true)  

  From the left menu, click on Service credentials. Click on View credentials to save the Username and Password somewhere safe for later use.  

  ![6](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/6.jpg?raw=true)  

### Step 3: Create Watson Studio Instance
- from Watson category in the IBM Cloud catalog, select **Watson Studio**.  

  ![7](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/7.jpg?raw=true)  
- Click **Create**.  

  ![8](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/8.jpg?raw=true)  

### Let's Get Started
- Click on **Get Started** to get redirected to Watson Studio Platform.  

  ![9](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/9.jpg?raw=true)  

- Create a **New Project**.  

  ![10](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/10.jpg?raw=true)

- Select **Complete** to include all available tools into the project.

  ![11](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/11.jpg?raw=true)
<br></br>


1. Enter a name for your project in the **Name:** field.
2. Associate the project **Storage** with the object storage instance you created in [step 1](###-Step-1:-Create-Object-Storage-Instance).
3. Click on **Create**.

    ![12](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/12.jpg?raw=true)

    Your project's **Assets** page will open.

    ![13](https://github.com/xnorax/watson-studio-journey/blob/master/imgs/13.jpg?raw=true)

## Contributers
- Nailah Al-Tayyar - Developer Advocate @IBM

## Credits
- [Watson Studio Enablement](https://github.com/HebaNAS/IBM-Watson-Studio-Enablement) for banking use case by Heba El-Shimy
- [Predictive Industrial Visual Analysis](https://github.com/IBM/Predictive-Industrial-Visual-Analysis) by IBM
