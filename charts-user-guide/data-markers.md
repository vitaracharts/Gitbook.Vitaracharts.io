# Data Markers

\


1. In traditional charts, data points are represented by bars and lines. Users of Vitara charts will be able to utilise markers to indicate the data points starting with version 4.4.
2. The markers menu offers a selection of data markers that you can choose from, or you can upload your own custom markers.
3.  The bar, column, line, area, sparkline, grid, and micro charts all have the data markers feature.

    **The following section will explain how to show a marker on the bar chart instead of bars.**

    In the vitara bar chart click on ‘Edit’ button to open the properties window.\
    \
    In the properties window open the ‘Series’ menu. Click on ‘Edit’ for the series on which you want to show the data markers.\
    \
    Expnad the ‘Type’ drop down box, and select the option ‘Data Markers’. When we select the option ‘Data Markers’, the series window will display all the options related to data markers.\
    \
    In the below screenshot the basic properties of the data markers like **marker selection, marker color and marker size** are highlighted.\


    **Marker Type, Marker Size and Marker Color**

    Click on the marker icon to open the marker selection window. Please refer to the below screenshot.\
    \
    After selecting the desired marker close the marker selection window. Select the size of the marker and color.\
    \
    Below is the screenshot of bar chart in which the bars are replaced with marker.\


    **Keep aspect ratio**

    When we enable data markers, we will see one marker for each data point. The position of the data marker is determined by the data point’s value. If we disable the Keep aspect ratio attribute, the data marker will be stretched to fill the space between the axis origin, i.e. 0, and the data point value.\


    Below is the screenshot of how the data markers looks when we disable **Keep Aspect ratio** property.\


    **Repeat Marker**

    In normal mode, one data marker is displayed for each data point. The data markers will be generated from a bar/column shape filled with markers when the Repeat Marker attribute is used. The marker will be filled with a certain number of rows inside each bar.\


    Enable the check box **Repeat Marker**.

    Select nummber of units per row. Click on apply.\
    \


**Fill**

If we choose **fill** mode, the data markers will be filled with a color depending on the value we set as Maximum value (while the marker size remains the same for all data points).

**Data markers as scatter chart**

Prior to 4.4, we could use the choices in the series tab to construct the scatter chart. We deleted the “Scatter” option from the “Series” menu in the 4.4 version. We may now use the “Data Markers” option to create scatter plots. The series-type drop down box will appear like this in the 4.4 release.\


Below are the steps to implement the scatter chart using the Vitara charts 4.4 version.\
**Step 1:** Use a Vitara Bar/column chart.

**Step 2:** In the “Appearance” tab, enable the option “Overlay Bar/Column”.\


**Step 3:** Open the “Series” tab and for the metric which you want to show as a simple tick, click on ‘Edit’.\


**Step 4:** Select the series type as “Data Markers”.\


**Step 5:** When we select the option ‘Data Markers’, the series window will display all the options related to data markers.\


**Step 6:** Click on “Apply” button.\


#### Custom SVG Markers <a href="#custom-svg-markers" id="custom-svg-markers"></a>

A new feature has been added to the 4.5 edition of vitara charts, allowing users to customise the data markers. This implies that the user can upload a local svg file to the server and use it as a data marker in Vitara charts. Custom svg markers can be used in the attributes of the following vitara charts:

```
        Series tab, 
        Markers tab, and 
        Thresholds tab.  
```

This feature is supported in the below charts.\
**Area, Bar, Bubble, Bullet, Column, Dumbbell, Histogram, Line, Simple KPI, Slope, Sparkline, Tornado, Trellis**, and **Waffle**.

Custom SVG markers can be used in the thresholds starting with Vitara Charts 4.6.1. The user can then submit the .svg file to the server and use it as a data marker in the Vitara Grid display.

Lets see how to use custom markers in the below steps. For better understanding of the process, we will consider the custom svg file as ‘**car.svg**’ in this example

**Step 1:**\
Upload an svg file \[**car.svg** in this case] into the server to this path in the plugins folder. {VitaraCharts/custom/images/}

**Step 2:**\
Create any chart \[line chart for example] that supports custom svg markers. Go to the marker tab, enable marker and click the ‘**marker type**’ icon, then the marker selection window will be opened. See the screenshot below.\


**Step 3:**\
Go to the **Custom** tab. Enter the name of the file in the **SVG path** textbox \[e.g, car.svg(name is case sensitive)] and click on ‘Apply’ and close the marked selection window. See the screenshot below\


Then the custom svg marker\[**car**] gets applied on the chart. see screenshot below\


In this way, the custom markers can be applied from the Series tab and Thresholds tab as well.

### Custom SVG markers in Data Labels <a href="#custom-svg-markers-in-data-labels" id="custom-svg-markers-in-data-labels"></a>

Custom svg markers are supported in data labels generated by thresholds, and various svg markers can be used to make the data labels more presentable to the applicable threshold.

The example below shows how to use ‘sun.svg’ as a custom marker on the threshold with data labels enabled.
