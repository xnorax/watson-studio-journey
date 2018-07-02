# Create an Interactive Dashboard

Analytics dashboard is a tool to build visualizations of your analytics results, communicate the insights that you've discovered and easily share the dashboard with others.

Click [here](https://dataplatform.ibm.com/dashboards/41a5bede-1e9d-4159-aa44-62e52715e6aa/view/6332c220259d29f062c7d4e407cc2e002f37775eb2bb850bd6847b495e687697f3384791c8274e528b170731f4e51551ca) to check out the Live Infographic that has been created in this tutorial.

## Create a Dashboard
1. From Watson Studio's main dashboard, select **New dashboard**.

    ![1](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/1.png)

- Type a name for your dashboard
- Select a **Congnos Dashboard Embedded Service** service instance. If you don't have one, you'll be prompted to create one then click reload to select it.
- Click **Save**.  
![2](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/2.png)

3. Select the template you wish to create, here I used an **Infographic** template.  
![3](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/3.png)

4. Select the page layout and click **Ok**.  
![4](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/4.png)

## Select Your Data Source
1. Click on **Selected sources**.  
![5](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/5.png)

2. We'll select **sensorData.csv** then click **Select**.

    ![6](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/6.png)

3. Click on the dataset to see all rows on the left panel.   
![7](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/7.png)

## Start Visualization
1. Select **Tempreture** and **avg_daily_output** columns and drag it where you want to place the visualization on the infographic template.

    *You can select multiple columns by pressing `Ctrl` while selecting the columns.*   
    ![8](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/8.png)

2. **Columns Chart** type will be automatically chosen based on the columns we selected.

    ![9](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/9.png)

3. If you need to edit the visualization, click on the crossing arrows on top of the visualization and then click on the visualization image from the side panel.  
![10](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/10.png)

4. To select another visualization method, select one from the listed options. Here, I click **More** for more options.  
![11](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/11.png)

5. Confirm the **Bar Chart** option to proceed.  
![12](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/12.png)

6. Insert **temperature** into the color property.  
![13](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/13.png)

6. Enter a title for your visualization. Choose the multimedia option from the left side-panel.  
![14](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/14.png)

7. Select the text option and drag it to where you want on the infographic template.  
![15](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/15.png)

8. Adding a title to the Infographic.  
![16](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/16.png)

9. You can choose **Properties** from the top toolbar to change the properties of any object in the visualization. Here I chose text properties.  
![18](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/18.png)

10. Changing the font weight, alignment and color.  
![18](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/19.png)

11. You can choose different themes for the visualization.  
![19](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/20.png)

12. Let's create another visualization. This time let's pick the `Rock categories` column from our dataset.  
![20](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/21.png)

13. Let's customize the visualization. I chose a **Pie Chart** for representing the different categories (summary ===> count) of the columns data. I chose to color the chart by `Rock categories` data as well, a differnt color for each category.  
![23](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/23.png)

    ![24](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/24.png)

14. Added a couple of other visualizations. You can try different styles.  
![29](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/25.png)

## Share Your Dashboard
1. After finishing the Infographic or the Dashboard, you can create a link to a **Read-Only** version of it and share it with anyone.

    ![30](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/26.png)

    Now you can see all visualizations are interactive!  
