# Create Pipeline Inspection Model Using Watson Visual Recognition

Watson Visual Recognition service on IBM Cloud enables you to tag, classify and search visual content using machine learning. We will use the service to create a custom model against a trained classifier to inspect oil and gas pipelines with six identifiers - Normal, Burst, Corrosion, Damaged Coating, Joint Failure and Leak in images.

## Steps
- [Step 1: Create Watson Visual Recognition Service](#step-1-create-watson-visual-recognition-service)
- [Step 2: Create Visual Recognition Model](#step-2-create-visual-recognition-model)
- [Step 3: Train Your Model](#step-3-train-your-model)
- [Step 4: Test Your Model](#step-4-test-your-model)

### Step 1: Create Watson Visual Recognition Service
1. From Watson Category in IBM Cloud Catalog, Click **Visual Recognition**.  
![1](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/1.jpg?raw=true)

2. Then click **Create**.

    *Note that _US-South_ region is recommended.*

    ![2](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/2.jpg?raw=true)


3. Now you have the service up and running.  
![3](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/3.jpg?raw=true)

### Step 2: Create Visual Recognition Model
1. Back to your project's **Assets** page in Watson Studio, Click **New visual recognition model**.  
![4](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/4.jpg?raw=true)

2. Make sure that Associated Service name matches your Watson Visual Recognition service that you recently created for things to run smoothly.

### Step 3: Train Your Model
1. Download the [training image dataset](https://github.com/xnorax/watson-studio-journey/tree/master/05-AnalyticsDashboard/training-image-dataset) and drag .zip files to your model.
![5](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/5.jpg?raw=true)

2. Select all datasets and click on **Add selected to model**.  
![6](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/6.jpg?raw=true)

3. Wait for a few minutes till the datasets are fully loaded. They will be added to separate classes based on the name of the zip files you provided. Now our model is ready for training, so let's hit **Train Model**.  
![7](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/7.jpg?raw=true)

4. Give Watson a few minutes to train the model on the provided images. Click on <span style="text-decoration:underline">here</span> from the top bar to view and test your model.
![8](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/8.jpg?raw=true)

### Step 4: Test Your Model
1. Click on **Test** tab.  
![9](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/9.jpg?raw=true)

2. Drag [sample images](https://github.com/xnorax/watson-studio-journey/tree/master/05-AnalyticsDashboard/sample-images) to test your model. In minutes, you'll see the model predicts which class each image belongs to.
![13](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/13.jpg?raw=true)

3. Also, you can test image from a file or link using REST API. Code samples can be found in **Implementation** tab.
![14](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/15.jpg?raw=true)

    There are different languages to help you integrate the model with your apps. You can also integrate it with Apple's Core ML to use your model on Apple's devices natively.
    ![14](https://github.com/xnorax/watson-studio-journey/blob/master/04-PipelineVisualRecognition/imgs/15.jpg?raw=true)
