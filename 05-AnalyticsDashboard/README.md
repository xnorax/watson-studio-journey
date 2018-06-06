# Create an Interactive Dashboard

Analytics dashboard is a tool to build visualizations of your analytics results, communicate the insights that you've discovered and easily share the dashboard with others.

Click [here](https://dataplatform.ibm.com/dashboards/55de357a-e905-4850-80aa-2260dc13be46/view/4503e47a20bf6fe24ad5c8e4079b7e052b3e2608b7bb8a52d5d07b495a607197f03c4796c82e4c5b8c405631f0e4110fcf) to check out the Live Infographic that has been created in this tutorial.

## Create a Dashboard
1. From Watson Studio's main dashboard, select **New Dashboard** from Dashboards panel.  
![1](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/1.png)

2. Type a name for your dashboard. Make sure you have a `dashboard analytics` service instance running and selected, if not you'll be prompted to create one then reload to select it. Click **Save**.  
![2](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/2.png)

3. Select the template you wish to create, here I used an Infographic template.  
![3](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/3.png)

4. Select the page layout and click **Ok**.  
![4](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/4.png)

## Select Your Data Source
1. Select a source for the data that will be used.  
![5](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/5.png)

2. We'll select our sensors data and click **Select**.   
![6](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/6.png)

3. Click on the dataset to expand it.We now see all the rows.   
![7](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/7.png)

## Start Visualization
1. Let's select columns for a visualization. You can select multiple columns by pressing `Ctrl` or `Cmd` while selecting the columns. Here, I selected `Tempreture` and `Avarage daily outcome`. Drag and drop your selected columns to where you want to place them on the infographic template.  
![8](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/8.png)

2. A visualization will be automatically picked for you, based on the data in the columns you selected. Here a **Columns Chart** was picked.  
![9](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/9.png)

3. If you need to edit the visualization, click on the crossing arrows on top of the visualization and a side panel will appear. Click on the visualization image as shown below.  
![10](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/10.png)

4. To select another visualization method, select one from the listed options. Here, I wanted more customization for the current visualization so click on **More**.  
![11](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/11.png)

5. Confirm the Bar Chart option to proceed.  
![12](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/12.png)

6. Now for making a better UI, let's choose a way to color the columns. Here, I picked coloring the columns according to the distinct of temperature we have, so I inserted `temperature` column into the color property.  
![13](https://github.com/xnorax/watson-studio-journey/blob/master/05-AnalyticsDashboard/imgs/13.png)

6. Let's enter a title for our visualization. Choose the multimedia option from the left side-panel.  
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
