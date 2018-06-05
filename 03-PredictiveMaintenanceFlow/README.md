# Build and compare models performances using IBM SPSS Modeler

A machine learning flow, which is a graphical representation of a data model, will be created throughout this tutorial  with drag-and-drop tooling from SPSS Modeler. We will use it to prepare data, train and compare between models.

## Create New Flow
From your project's **Assets** page, Click **New flow**.

  ![1](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/1.jpg?raw=true)

1. Type a name and description for your machine learning flow.
2. Select **Modeler Flow** as the flow type.
3. Select **IBM SPSS Modeler** as a runtime environment.
4. Click **Create**.

    ![2](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/2.jpg?raw=true)

## Adding Data
1. From the **Flow Editor** toolbar, click the Open Palette icon(![icon](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/open_palette.png?raw=true)).
2. Add a **Data Asset** node from the *Import* category in the palette.

    ![4](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/4.jpg?raw=true)

3. Double click the node to open the editor then click **Change Data Asset**.

    ![5](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/5.jpg?raw=true)

4. A list of available data assets in your project will be opened. Select the *sensorTrainingData* dataset and click **OK**.

      ![6](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/6.jpg?raw=true)

7. Then click **Save** in the node editor to apply your changes.

    ![7](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/7.jpg?raw=true)

## Explore Data
1. Drag **Data Audit** node to the canvas.

    > Data Audit provides a comprehensive first look at the data, including summary statistics, histograms and distribution for each field, as well as information about outliers, missing values, and extremes. Results are displayed in an easy-to-read matrix that can be sorted and used to generate full-size graphs and data preparation nodes.

    ![8](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/8.jpg?raw=true)

2. Connect the **Data Asset** and **Data Audit** nodes.  

    ![10](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/9.jpg?raw=true)

3. Right-click on the data audit node, then click on **Run**.  

    ![11](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/10.jpg?raw=true)

4. Wait for the process to finish.  

    ![12](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/11.jpg?raw=true)

5. In the right-side panel, under the **Outputs** tab, let's select the most recent output (most recent is always on top) to view the results of running the flow so far.  

    ![12](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/12.jpg?raw=true)

6. We get an idea about some statistics of the data and the distribution of the features. We find that the data needs some kind of normalization.  

    ![13](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/13.jpg?raw=true)

7. Let's go back to our Modeler and continue working there.  

    ![14](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/14.jpg?raw=true)

## Split Data
1. Drag **Partition** node to split the data into separate training and testing subsets.

    ![16](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/15.jpg?raw=true)

2. Double-clicking on the **Partition** node to explore its properties. We'll leave everything as it is.  
![17](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/16.jpg?raw=true)

## Prepare Data
We'll add **Auto Data Prep** to automatically find issues in our dataset and fix it.  
![18](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/17.jpg?raw=true)

## Explore Data Again
1. We'll do another **Data Audit** to check the results of the previous step.  
![19](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/18.jpg?raw=true)

2. View the results.  
![20](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/19.jpg?raw=true)

3. The data has been normalized and issues have been fixed.  
![21](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/20.jpg?raw=true)

## Add Prediction Model
1. Now let's select a model, let's try **C&R Tree**.  
![22](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/21.jpg?raw=true)

2. Double-clicking on the **C&R** node to change its properties. Check **Use custom field roles**, then select `Target_transformed` as the target(labels) column and select all other columns as **Inputs**. Click **Save**.  
![23](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/22.jpg?raw=true)

3. Let's run the flow.  
![24](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/23.jpg?raw=true)

4. Wait for the process to finish. It may take a few minutes.  
![25](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/24.jpg?raw=true)

5. After the model runs, it will produce a new node that holds information about the performance of the model.  
![26](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/25.jpg?raw=true)

## Analyze Results
1. Let's add an **Analysis** node to peek into the model results node.  
![27](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/26.jpg?raw=true)

2. Connect the nodes.  
![28](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/27.jpg?raw=true)

3. View the output.  
![29](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/27.jpg?raw=true)

4. Information about how our model performed.  
![30](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/28.jpg?raw=true)

## Compare Models
1. I added a few other models for comparison. Feel free to try your own combinations.  
![31](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/29.jpg?raw=true)

2. If we click on the **C&R Tree** model node again and choose **View model**, we will get more detailed information about different performance metrics.  
![36](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/30.jpg?raw=true)

    ![37](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/31.jpg?raw=true)

    ![38](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/32.jpg?raw=true)

    ![39](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/33.jpg?raw=true)

3. Checking another model's performance (LSVM) as we did in the previous step.  
![32](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/34.jpg?raw=true)

    ![33](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/35.jpg?raw=true)

    ![34](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/36.jpg?raw=true)

    ![35](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/37.jpg?raw=true)

4. We're satisfied with our second model, it has better overall performance. Let's click on its node **LSVM** and select **Save branch as model**.  
![38](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/38.jpg?raw=true)

5. Type a name for your model and a machine learning service should be detected and added automatically. Then click **Save**.  

    ![39](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/39.jpg?raw=true)

6. The model has been saved successfully.  

    ![40](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/40.jpg?raw=true)

7. You can access it in the Models panel in the main dashboard.  

    ![41](https://github.com/xnorax/watson-studio-journey/blob/master/03-PredictiveMaintenanceFlow/imgs/41.jpg?raw=true)


You can easily iterate through these steps and do some tweaks in the configuration options of each step/node to achieve better accuracy.
